<script setup>
const columns = [
  {
    name: 'lastAction',
    required: true,
    label: 'Последняя активность ',
    field: 'lastAction',
    align: 'left',
    sortable: true,
  },
  { name: 'calories', align: 'left', label: 'Состав', field: 'customers', sortable: true },
  { name: 'tel', align: 'left', label: 'Номер телефона', field: 'tel' },
  { name: 'carbs', align: 'left', label: 'Жилой комплекс', field: 'carbs' },
  { name: 'protein', label: 'Protein (g)', field: 'protein' },
  { name: 'sodium', label: 'Sodium (mg)', field: 'sodium' },
  {
    name: 'calcium',
    label: 'Номер телефона',
    field: 'calcium',
    sortable: true,
    sort: (a, b) => parseInt(a, 10) - parseInt(b, 10),
  },
]

const rows = [
  {
    lastAction: '20.06.2024',
    customers: 'Васильев В. В. Васильева В. В.',
    tel: '+7 900 123 12 12',
    carbs: 'Б15',
    protein: 'Ипотека',
    sodium: 'Петрова А. Ф.',
    calcium: 'Активно',
  },
]
</script>
<template>
  <div class="q-pa-md">
    <q-table title="Treats" :rows="rows" :columns="columns" row-key="name"></q-table>
  </div>
</template>
