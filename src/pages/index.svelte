<script>
  import { acak } from "kumpulan-tools";
  import semua_crypto from "../data/crypto";

  let terpilih;
  function pilih() {
    terpilih = acak(semua_crypto)[0];
  }
  pilih();
</script>

<div class="min-h-screen w-full grid grid-cols-1 content-around">
  <div class="text-center text-3xl">{terpilih}</div>
  <div>
    <button
      class="bg-black text-white px-4 py-2 rounded mx-auto block"
      on:click={pilih}>Acak</button
    >
  </div>
</div>
