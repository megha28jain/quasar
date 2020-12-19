<template>
  <q-page class="flex">
    <div class="flex-row">
      Quasar Flex CSS classes can be applied based on the width of the screen, to help you in making a responsive UI. The 12 points grid is inspired by Bootstrap’s, so there are a lot of similarities.<br/>
      What we’ve learned so far is that, for example, we can size the columns regardless of window width. If we are to create a responsive UI, we need to dynamically change the sizing while taking window width into account.<br/>
      First, let’s learn about some tokens that you<br/>
      Quasar Flex CSS classes can be applied based on the width of the screen, to help you in making a responsive UI. The 12 points grid is inspired by Bootstrap’s, so there are a lot of similarities.
      What we’ve learned so far is that, for example, we can size the columns regardless of window width. If we are to create a responsive UI, we need to dynamically change the sizing while taking window width into account.<br/>
      First, let’s learn about some tokens that you
    </div>
    <div class="flex-column">
      <div class="q-pa-md items-start q-gutter-md">
        <q-card flat bordered class="my-card">
          <q-card-section>
            <q-item-label header class="text-h6">Fundraising progress</q-item-label>
            <div class="flex justify-between">
              <div class="flex-column example-cell">
                <div>Commited</div>
                <div>$650,000</div>
              </div>
              <div class="flex-column example-cell">
                <div>Minimum Goal</div>
                <div>$2,000,000</div>
              </div>
            </div>
            <div class="q-pa-md">
              <q-linear-progress size="10px" :value="progress" />
            </div>
            <div>32 investors in process<br/>Closes by 30 Nov 2020</div>
          </q-card-section>
        </q-card>
      </div>
      <div class="q-pa-md row items-start q-gutter-md">
        <q-card flat bordered class="my-card">
          <q-card-section>
            <div class="q-px-lg q-pb-md">
              <q-timeline color="orange">
                <q-timeline-entry heading>
                  Investment process
                </q-timeline-entry>

                <q-timeline-entry
                  title="Initialise commitment"
                >
                  <div>
                    View key terms and enter an investment amount, which will be confirmed by the project team in less than a business day.<br/>
                    <b color="orange">Open for commitment until 22 Nov </b>
                    <div class="q-pa-md q-gutter-sm">
                      <q-btn color="deep-orange" glossy label="View key terms" />
                    </div>
                  </div>
                </q-timeline-entry>

                <q-timeline-entry
                  title="Investor call"
                >
                  <div>
                    Join a Zoom call with the project team, lead investor and co-investors.
                  </div>
                </q-timeline-entry>

                <q-timeline-entry
                  title="Sign investment agreement"
                >
                  <div>
                    View final investment agreement and sign digitally. Evident will collect other signatures within 3 business days to finalise the contract.
                  </div>
                </q-timeline-entry>

                <q-timeline-entry
                  title="Payment"
                >
                  <div>
                    Send your investment via bank transfer,which will be confirmed by the project team in less than a business day.
                  </div>
                </q-timeline-entry>

                <q-timeline-entry
                  title="Completion"
                >
                  <div>
                    Project updates and reports will be available in Portfolio.
                  </div>
                </q-timeline-entry>
              </q-timeline>
            </div>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      progress: 0.4
    }
  }
}
</script>

<style lang="sass" scoped>
  .example-cell
    margin: 1px
    padding: 4px 8px
    box-shadow: inset 0 0 0 2px $grey-6
</style>
