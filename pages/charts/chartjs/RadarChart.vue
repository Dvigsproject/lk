<script>
import { Radar } from 'vue-chartjs'

export default {
  extends: Radar,
  mounted() {
    this.renderChart(
      {
        labels: [
          'Eating',
          'Drinking',
          'Sleeping',
          'Designing',
          'Coding',
          'Cycling',
          'Running',
        ],
        datasets: [
          {
            label: 'Desktops',
            backgroundColor: 'rgba(59, 175, 218,0.2)',
            borderColor: '#1aad9c',
            pointBackgroundColor: '#1aad9c',
            pointBorderColor: '#fff',
            pointHoverBackgroundColor: '#fff',
            pointHoverBorderColor: '#1aad9c',
            data: [65, 59, 90, 81, 56, 55, 40],
          },
          {
            label: 'Tablets',
            backgroundColor: 'rgba(246, 114, 167,0.2)',
            borderColor: '#f672a7',
            pointBackgroundColor: '#f672a7',
            pointBorderColor: '#fff',
            pointHoverBackgroundColor: '#fff',
            pointHoverBorderColor: '#f672a7',
            data: [28, 48, 40, 19, 96, 27, 100],
          },
        ],
      },
      {
        maintainAspectRatio: true,
        legend: {
          position: 'top',
        },
      }
    )
  },
}
</script>
