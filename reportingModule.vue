<template>
    <q-page class="q-pa-md" >
        <q-list
          bordered
          v-for="lpr in lprData"
          :key="lpr.id"
          class="">
            <q-item>
                <q-item-section avatar>
                    <q-icon name="speed" color="blue" size="34px" />
                </q-item-section>

                <q-item-section>
                    <q-item-label lines="1" class="text-weight-bold text-primary">
                        <span class="q-pa-lg">{{ lpr.id }}</span>
                        <span class="q-pa-lg">{{ lpr.plate_number }}</span>
                        <span class="q-pa-lg">{{ lpr.country }}</span>
                        <span class="q-pa-lg">{{ lpr.date_time }}</span>
                        <span class="q-pa-lg"> {{ lpr.speed /100 }} KM/h </span>
                    </q-item-label>
                </q-item-section>

                <!-- Action Buttons -->
                <q-item-section top side>
                    <div class="text-grey-8 q-gutter-xs">
                        <q-btn class="" size="12px" flat dense round icon="print" />
                        <q-btn class="" size="12px" flat dense round icon="done" />
                        <q-btn class="" size="12px" flat dense round icon="undo" />
                    </div>
                </q-item-section>
            </q-item>
        </q-list>


    </q-page>
</template>
<script>
export default {
    data() {
        return {
            moduleName: 'reporting-module',
            lprData: [
                {
                    id: 249,
                    device_name: "10417",
                    plate_number: "‭١٤٩‬‭ص‌ر‌م‬",
                    country: "EGY",
                    date_time: "2019-07-30, 13:56:31",
                    speed: "1192"
                },
                {
                    id: 250,
                    device_name: "10417",
                    plate_number: "‭١٤٩‬‭ص‌ر‌م‬",
                    country: "EGY",
                    date_time: "2019-07-30, 13:56:31",
                    speed: "1192"
                }
            ]
        }
    },
    components: {
    }
}
</script>
