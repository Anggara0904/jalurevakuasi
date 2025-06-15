<script setup>
import { Button } from "@/components/ui/button";
import {
  Table,
  TableBody,
  TableCaption,
  TableCell,
  TableHead,
  TableHeader,
  TableRow,
} from "@/components/ui/table";
import { RouterLink } from "vue-router";
</script>

<template>
  <section class="">
    <div
      class="mx-auto flex min-h-screen max-w-screen-lg flex-col items-center justify-center gap-y-4 px-4 py-8"
    >
      <h1 className="text-center text-3xl font-bold uppercase">
        Kontak Darurat Brebes Selatan
      </h1>
      <h2 className="my-2 text-center text-lg font-medium capitalize">
        Kontak darurat yang bisa dihubungi Kecamatan yang berada di Brebes Selatan
      </h2>
      <div class="w-full bg-slate-50">
        <Table class="font-medium">
          <TableCaption>
            Siaga Darurat di Brebes Selatan: Pastikan Anda selalu siap
            menghadapi segala situasi darurat dengan menyimpan nomor kontak
            penting ini! Ketika bencana melanda atau situasi genting terjadi,
            bantuan cepat dan tepat sangat dibutuhkan. Jangan panik, hubungi
            layanan darurat yang siap siaga untuk memberikan pertolongan pertama
            dan bantuan yang Anda perlukan. Keselamatan Anda adalah prioritas
            kami!
          </TableCaption>
          <TableHeader>
            <TableRow>
              <TableHead class="w-[100px] font-bold">No</TableHead>
              <TableHead class="font-bold">Desa</TableHead>
              <TableHead class="font-bold">Kontak</TableHead>
            </TableRow>
          </TableHeader>
          <TableBody>
            <TableRow>
              <TableCell class="font-medium">01</TableCell>
              <TableCell>Paguyangan</TableCell>
              <TableCell>
                <a class="text-yellow-600 underline" href="tel:082190054717">
                  082190054717
                </a>
              </TableCell>
            </TableRow>
            <TableRow>
              <TableCell class="font-medium">02</TableCell>
              <TableCell>Bumiayu</TableCell>
              <TableCell>
                <a class="text-yellow-600 underline" href="tel:082211502256">
                  082211502256
                </a>
              </TableCell>
            </TableRow>
            <TableRow>
              <TableCell class="font-medium">03</TableCell>
              <TableCell>Tonjong</TableCell>
              <TableCell>
                <a class="text-yellow-600 underline" href="tel:081244263899">
                  081244263899
                </a>
              </TableCell>
            </TableRow>
            <TableRow>
              <TableCell class="font-medium">04</TableCell>
              <TableCell>Sirampog</TableCell>
              <TableCell>
                <a class="text-yellow-600 underline" href="tel:081342581898">
                  081342581898
                </a>
              </TableCell>
            </TableRow>
            <TableRow>
              <TableCell class="font-medium">05</TableCell>
              <TableCell>Bantarkawung</TableCell>
              <TableCell>
                <a class="text-yellow-600 underline" href="tel:0812445616569">
                  081244561656
                </a>
              </TableCell>
            </TableRow>
            <TableRow>
              <TableCell class="font-medium">06</TableCell>
              <TableCell>Salem</TableCell>
              <TableCell>
                <a class="text-yellow-600 underline" href="tel:081244265465">
                  081244265465
                </a>
              </TableCell>
            </TableRow>
          </TableBody>
        </Table>
      </div>
      <Button
        class="flex items-center justify-center gap-1"
        :as="RouterLink"
        to="/"
      >
        <v-icon name="fa-arrow-left" />
        Kembali
      </Button>
    </div>
  </section>
</template>
