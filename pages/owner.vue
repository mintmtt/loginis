<template>
  <v-row justify="center">
    <v-col cols="12" sm="3">
      <v-row
        ><v-col cols="12" sm="12">
          <v-card rounded="lg" min-height="150" color="white">
            <v-toolbar color="green" dark dense flat>
              <v-toolbar-title class="body-3">
                จำนวนรถยนต์ที่ว่าง
              </v-toolbar-title>
            </v-toolbar>
            <v-card-text> มีจำนวนทั้งหมด </v-card-text>
            <v-col class="text-center" cols="12">
              <v-list-item-title>6 คัน</v-list-item-title>
            </v-col>
          </v-card>
        </v-col>
        <v-col cols="12" sm="12">
          <v-card rounded="lg" min-height="150" color="white">
            <v-toolbar color="red" dark dense flat>
              <v-toolbar-title class="body-3">
                จำนวนรถยนต์ที่อยู่ระหว่างเช่า
              </v-toolbar-title>
            </v-toolbar>
            <v-card-text> มีจำนวนทั้งหมด </v-card-text>
            <v-col class="text-center" cols="12">
              <v-list-item-title>4 คัน</v-list-item-title>
            </v-col>
          </v-card>
        </v-col></v-row
      >
    </v-col>

    <v-col cols="12" sm="8">
      <v-card rounded="lg" min-height="500" color="white">
        <v-toolbar color="yellow" dense flat>
          <v-toolbar-title class="body-3">
            จำนวนรายรับรายเดือน
          </v-toolbar-title>
        </v-toolbar>
        <v-simple-table height="450">
          <template v-slot:default>
            <thead>
              <tr>
                <th class="text-left">Name</th>
                <th class="text-left">Income</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="item in desserts" :key="item.name">
                <td>{{ item.name }}</td>
                <td>{{ item.calories }}</td>
              </tr>
            </tbody>
          </template>
        </v-simple-table>
        <v-footer padless>
          <v-col class="text-center" cols="8">
            <v-list-item-title>All</v-list-item-title>
          </v-col>
          <v-col class="text-center" cols="4">
            <v-list-item-title class="text-left">500000 บาท</v-list-item-title>
          </v-col>
        </v-footer>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      desserts: [
        {
          name: 'Frozen Yogurt',
          calories: 159,
        },
        {
          name: 'Ice cream sandwich',
          calories: 237,
        },
        {
          name: 'Eclair',
          calories: 262,
        },
        {
          name: 'Cupcake',
          calories: 305,
        },
        {
          name: 'Gingerbread',
          calories: 356,
        },
        {
          name: 'Jelly bean',
          calories: 375,
        },
        {
          name: 'Lollipop',
          calories: 392,
        },
        {
          name: 'Honeycomb',
          calories: 408,
        },
        {
          name: 'Donut',
          calories: 452,
        },
        {
          name: 'KitKat',
          calories: 518,
        },
      ],
    }
  },
}
</script>
<style>
.card {
  max-width: 300px;
  width: 450px;
  margin: 10px;
}
.img {
  min-height: 200px;
  min-width: 300px;
}
</style>