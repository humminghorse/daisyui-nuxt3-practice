<template>
  <div class="card w-1/3 bg-base-100 h-auto mt-2 shadow-xl">
    <figure class="px-2 pt-2">
      <img src="coordinationImgSrc" class="rounded-xl" />
    </figure>
    <div class="card-body items-center text-center">
      <h3 class="text-sm -ml-24 -mt-4">着用中のアイテム</h3>
      <div class="flex items-center">
        <img src="itemImgSrc" class="rounded-xl h-12" />
        <p class="text-sm ml-4">
          {{ itemName }}<br />(カラー: {{ itemColor }})
        </p>
      </div>
      <div class="card-actions mt-2">
        <button class="btn btn-primary w-full">
          アイテムの<br />詳細を見る
        </button>
        <button class="btn btn-primary w-full">
          この子の<br />他のコーディネートを見る
        </button>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
type Props = {
  coordinationImgSrc: string;
  itemImgSrc: string;
  itemName: string;
  itemColor: string;
};
export default defineComponent({
  props: {
    coordinationImgSrc: {
      type: String,
      required: true,
    },
    itemImgSrc: {
      type: String,
      required: true,
    },
    itemName: {
      type: String,
      required: true,
    },
    itemColor: {
      type: String,
      required: true,
    },
  },
});
</script>
