<template>
    <div class="upcoming">
        <h4>Wanna transform you life?</h4>
        <h1>Upcoming Events</h1>
        <div class="container-event">
            <div class="card-event" v-for="event in events" :key="event.id">
                <div class="location">
                    <div>
                        <i class="fas fa-map-marker-alt"></i>
                        <span>{{event.location}}</span>
                        </div>
                        <h5>{{event.title}}</h5>
                    </div>
                <div class="date-event">
                    <h1>{{event.day}}</h1>
                    <p>{{event.month}}</p>
                    <div class="get-ticket">Get ticket</div>
                </div>
            </div>
        </div>
        <div class="all-event">
            <span class="pr-5">Excited about our event?</span>
            <span class="green">View all events &#8594;</span>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        events:Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
    .upcoming{
        height: 700px;
        .all-event{
            text-align: center;
            font-weight: 600;
            .green{
                color: $jungle-green;
                border-bottom: 1px solid $silver;
            }
        }
        h4{
            color: $jungle-green-v;
            text-align: center;
            padding-top: 50px;
            padding-bottom: 30px;
        }
        h1{
            text-align: center;

        }
        .container-event{
            display: flex;
            padding-bottom: 50px;
            padding-top: 30px;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            width: 820px;
            margin: 0 auto;
            .card-event{
                width: 400px;
                height: 130px;
                padding-top: 20px;
                padding-left: 20px;
                display: flex;
                justify-content: space-between;
                background-color: $link-water;
                border-radius: 5px;
                .location{
                    gap: 5px ;
                    padding-bottom: 5px;
                    display: flex;
                    flex-direction: column;
                      i{
                    color: grey;
                }
                span{
                    font-size: 12px;
                    padding-left: 5px;
                }
                }
              .date-event{
                  padding-right: 50px;
                  display: flex;
                  flex-direction: column;
                  h1{
                      font-weight: 500;
                      color: $jungle-green-v;
                  }
                  p{
                      font-weight: 600;
                      font-size: 12px;
                      text-align: center;
                  }
                  .get-ticket{
                      width: 130px;
                      height: 30px;
                      background-color: $jungle-green-v;
                      color: $white;
                      line-height: 30px;
                      text-align: center;
                      font-size: 12px;
                      border-radius: 5px;
                      margin-top: 5px;
                      &:hover{
                          background-color: $tuna;
                      }
                  }
              }
            }
        }
    }
</style>