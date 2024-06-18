<div id="app">
  <table>
    <thead>
      <tr>
        <th>Country</th>
        <th>Currency Code (ISO)</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(currency, country) in currencyList" :key="country">
        <td>{{ country }}</td>
        <td>{{ currency }}</td>
      </tr>
    </tbody>
  </table>
</div>

<script src="https://cdn.jsdelivr.net/npm/vue@2.6.14/dist/vue.js"></script>
<script>
  new Vue({
    el: '#app',
    data: {
      currencyList: {}
    },
    mounted() {
      fetch('https://westinpay.com/currency/fiat_api?api_key=YOUR-API-KEY&base=USD&output=JSON')
        .then(response => response.json())
        .then(data => {
          this.currencyList = data.rates;
        })
        .catch(error => {
          console.error('Error fetching currency rates:', error);
        });
    }
  });
</script>
