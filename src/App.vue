<script setup>
import { h } from 'vue'
import { format } from 'date-fns'
import TabelPiutang from '@/components/TabelPiutang.vue'
import dataPiutang from '@/dataPiutang.json'
import RefreshPage from '@/components/RefreshPage.vue'
const columnsPiutang = [
  {
    accessorKey: 'noKe',
    header: 'No. Kewajiban',
  },
  {
    accessorKey: 'noPolis',
    header: 'No. Polisi',
  },
  {
    accessorKey: 'pemilik',
    header: 'Pemilik',
  },
  {
    accessorKey: 'peserta',
    header: 'Peserta',
  },
  {
    accessorKey: 'noVA',
    header: 'Nomor VA',
  },
  {
    accessorKey: 'hgTer',
    header: 'Harga Terbentuk',
  },
  {
    accessorKey: 'bAdmin',
    header: 'Biaya Admin Ex PPN',
  },
  {
    accessorKey: 'ppn',
    header: 'PPN',
  },
  {
    accessorKey: 'total',
    header: 'Total',
  },
  {
    accessorKey: 'tgLelang',
    header: 'Tanggal Lelang',
  },
  {
    accessorKey: 'tgJtTempo',
    header: 'Tanggal Jatuh Tempo',
  },
  {
    accessorKey: 'tgLunas',
    header: 'Tanggal Lunas',
  },
  {
    accessorKey: 'status',
    header: 'Status',
  },
]
</script>

<template>
  <div class="container px-8 py-8">
    <h2 class="text-center text-2xl">Daftar Piutang Unit</h2>
    <div class="my-8">
      
      <TabelPiutang :data="dataPiutang" :columns="columnsPiutang" />
    </div>
  </div>
</template>


