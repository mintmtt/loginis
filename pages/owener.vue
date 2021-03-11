<template>
  <v-row dense>
    <v-col cols="6">
      <v-card color="#385F73" dark>
        <v-card-title class="headline"> รถว่าง </v-card-title>
        <v-divider class="mx-4"></v-divider>
        <v-card-subtitle>จำนวน 7 คัน</v-card-subtitle>
      </v-card> </v-col
    ><v-col cols="6">
      <v-card color="#385F73" dark>
        <v-card-title class="headline"> รถที่ถูกจอง </v-card-title>
        <v-divider class="mx-4"></v-divider>
        <v-card-subtitle>จำนวน 3 คัน</v-card-subtitle>
      </v-card>
    </v-col>
    <v-col cols="12">
      <v-card>
        <v-tabs fixed-tabs background-color="indigo" dark>
          <v-tab v-for="item in items" :key="item"> {{ item }}</v-tab>
        </v-tabs>
        <v-divider class="mx-4"></v-divider>
        <v-card-subtitle>รวมทั้งหมด {{ text }}</v-card-subtitle>
        <v-divider class="mx-4"></v-divider>
        <v-card-subtitle>{{ text }}</v-card-subtitle></v-card
      >
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    title: 'rental',
    items: ['ยอดการจองรายเดือน', 'ยอดการจองรายปี'],
    text: '30000',
  }),
}
</script>