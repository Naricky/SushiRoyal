<template>
  <div class='background'>
    <div class='table'>
      <a>
        <tr class='openHour'>OPENING HOUR</tr>
      </a>
      <table class="table-plain branch-hours">
        <tbody class="line">
          <tr class="Monday">
            <td>Monday: </td>
            <td>11:00am-10:00pm</td>
          </tr>
          
          <tr class="Tuesday">
            <td>Tuesday: </td>
            <td>11:00am-10:00pm</td>
          </tr>

          <tr class="Wednesday">
            <td>Wednesday: </td>
            <td>11:00am-10:00pm</td>
          </tr>

          <tr class="Thursday">
            <td>Thursday: </td>
            <td>11:00am-10:00pm</td>
          </tr>

          <tr class="Friday">
            <td>Friday: </td>
            <td>11:00am-10:00pm</td>
          </tr>

          <tr class="Saturday">
            <td>Saturday: </td>
            <td>11:00am-10:00pm</td>
          </tr>

          <tr class="Sunday">
            <td>Sunday: </td>
            <td>11:00am-10:00pm</td>
          </tr>

        </tbody>
      </table>
    </div>
    <div class='other'>
      <a class='phoneAndAddress'> Phone Number and Address </a>
        <div class='phone'>
          604-568-4500 /
          604-558-4994
        </div>
        <div class='address'>
          82 Keefer Place (across International Village), Vancouver, BC, V6B 0C9
        </div>
    </div>
  </div>
</template>

<script>
export default {

}

</script>

<style scoped>

.phone, .address {
  text-align: center;
}

.table {
  width: 50%;
  float: left;
  text-align: center;
}

.other {
  width: 50%;
  float: right;
  text-align: center;
  background-color: white;
  font-family: "AvenirNextLTW01-Regular", sans-serif;
  font-size: 16;
  line-height: 1.3;
  color: #bcbcbc;
}

.openHour {
  color: #bcbcbc;
}

.phoneAndAddress {
  text-align: center;
}

a {
  color: #d8964c;
  font-family: 'TradeGothicW01-Extended', sans-serif;
  text-transform: uppercase;
  margin: 0;
  font-size: 30px;
  margin-bottom: 20px;
}

.background {
  text-align: center;
}

table.table-plain,
table.table-plain td
{
    border: none !important;
    /*table-layout: auto;*/
    /*padding: .5rem;*/
    padding: 0;
    /*border-spacing: 0;*/
    font-family: "AvenirNextLTW01-Regular", sans-serif;
    font-size: 16;
    line-height: 1.5;
    color: #bcbcbc;
    margin-bottom: 20px;
    width: 100%;
    max-width: 400px;
    text-align: center;
}

table.table-plain td:first-child {
  text-align: center;
  font-weight: bold;
  width: 70%;

}

table.table-plain td:nth-child(2) {
  text-align: center;
}

#contact > div > div.table {
  background-color: #111111;
}

.line {
  text-align: center;
}

tr {
  text-align: center;
}

</style>
