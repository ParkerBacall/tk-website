<template>
    <div class='home-body'>
        <div :class="[$vuetify.breakpoint.mdAndUp ? 'body-1' : 'body-2']" class='mission-statement'> From Roots to Wings exists to helps develop communities by following the lead of community members and leaders something something</div>
        <HomeTimeline />
        <!-- <div class="stat-title headline">
            Out of 1,239 Families Surveys
        </div>
        <div class="stat-card-container">
            <v-card
            class="mx-auto stat-card-outter"
            max-width="344"
            flat
            >
            <v-card-text class="stat-card-inner">
                <div class="card-text body-1">
                Families Making Less Than<br>
                $80.00 a Month
                </div>
                <v-progress-circular
                    class="stat-progress"
                    :rotate="360"
                    :size="100"
                    :width="15"
                    :value="incomeValue"
                    color="light-blue accent-3"
                >
                    {{incomeValue}}%
                </v-progress-circular>
            </v-card-text>
            <v-card-actions>
                <v-btn
                text
                color="deep-purple accent-4"
                >
                Learn More
                </v-btn>
            </v-card-actions>
            </v-card>
            <v-card
            class="mx-auto stat-card-outter"
            max-width="344"
            flat
            >
            <v-card-text class="stat-card-inner">
                <div class="card-text body-1">
                Children Not<br>
                in School
                </div>
                <v-progress-circular
                    class="stat-progress"
                    :rotate="360"
                    :size="100"
                    :width="15"
                    :value="schoolValue"
                    color="light-blue accent-3"
                >
                    {{schoolValue}}%
                </v-progress-circular>
            </v-card-text>
            <v-card-actions>
                <v-btn
                text
                color="deep-purple accent-4"
                >
                Learn More
                </v-btn>
            </v-card-actions>
            </v-card>
        </div> -->
        <AmazonSmile />
    </div>  
</template>

<script>
import HomeTimeline from './HomeTimeline.vue'
import AmazonSmile from './AmazonSmile.vue'

export default {
    components: {
        HomeTimeline,
        AmazonSmile
    }
}
</script>

<style>
.home-body {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.mission-statement.body-2{
    text-align: center;
    width: 90%;
    margin-top: 1rem;
    font-weight: 300;
}

.mission-statement.body-1{
    text-align: center;
    width: 30%;
    margin-top: 2rem;
}

/* .mission-statement{
    text-align: center;
    margin-top: 1rem;
    font-size: 15pt;
    width: 30%;
    font-weight: 300;
} */

.card-text{
    text-align: center;
    line-height: 2rem;
    color: #000000;
}


</style>