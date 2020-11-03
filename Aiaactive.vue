<template>
<div class="q-pa-md q-gutter-md">
    <q-list v-for="lpr in lprData" :key="lpr.id" bordered class="rounded-borders" style="lprData.style">
        <q-item>
            <q-item-section avatar>
                <q-icon name="speed" color="blue" size="34px" />
            </q-item-section>

            <q-item-section>
                <q-item-label lines="1" class="q-pa-xs text-body2 text-weight-bold text-primary text-uppercase">
                    <span class=" q-pa-xl cursor-pointer">{{ lpr.id }}</span>
                    <span class=" q-pa-xl cursor-pointer">{{ lpr.plate_number }}</span>
                    <span class="q-pa-xl cursor-pointer">{{ lpr.country }}</span>

                    <span class="q-pa-xl cursor-pointer">{{ lpr.date_time }}</span>

                    <span class="q-pa-xl cursor-pointer"> {{ lpr.speed }} </span>
                </q-item-label>
            </q-item-section>

            <!-- Action Buttons -->
            <q-item-section top side>
                <div class="text-grey-8 q-gutter-xs">
                    <q-btn class="gt-xs" size="12px" flat dense round icon="print" />
                    <q-btn class="gt-xs" size="12px" flat dense round icon="done" />
                    <q-btn class="gt-xs" size="12px" flat dense round icon="undo" />
                </div>
            </q-item-section>
        </q-item>
    </q-list>
</div>
</template>

<script>
export default {
    data() {
        return {
            lprData: [{
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
        };
    }
};
</script>
