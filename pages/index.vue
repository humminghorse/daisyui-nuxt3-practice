<template>
  <!-- 参考: このページを真似している https://wear.jp/coordinate/?tag_ids=600 -->
  <!-- 参考: containerクラス https://tailwindcss.jp/docs/container#app -->
  <div class="container mx-auto pl-4 pr-4 bg-white">
    <TheHeader />
    <div class="tabs tabs-boxed w-full">
      <a class="tab w-1/4 tab-active">コーディネート</a>
      <a class="tab w-1/4">ペット</a>
      <a class="tab w-1/4">アイテム</a>
      <a class="tab w-1/4">ショップ</a>
    </div>
    <div class="border-b-2">
      <h1 class="mt-4 text-2xl">コーディネート一覧</h1>
      <p class="mt-2 text-right">211件</p>
    </div>

    <!-- body -->
    <div class="flex bg-neutral">
      <div class="control-panel bg-white flex-auto m-4 p-2 w-1/4">
        <h3 class="text-lg mt-2">ペットの種類</h3>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-pet-type"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">犬</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-pet-type"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">猫</span>
          </label>
        </div>
        <h3 class="text-lg mt-2">ペットの色</h3>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-pet-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">白</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-pet-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">黒</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-pet-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">茶</span>
          </label>
        </div>
        <h3 class="text-lg mt-2">アイテムの種類</h3>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-type"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">首輪</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-type"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">服</span>
          </label>
        </div>
        <h3 class="text-lg mt-2">アイテムの色</h3>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">白</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">黒</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">赤</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">青</span>
          </label>
        </div>
        <div class="form-control">
          <label class="label cursor-pointer justify-start">
            <input
              type="radio"
              name="radio-item-color"
              class="radio checked:bg-accent mr-2"
              checked
            />
            <span class="label-text">黄</span>
          </label>
        </div>
      </div>
      <div class="content flex-auto mx-4 my-4 h-128 w-1/2"></div>
    </div>

    <TheFooter />
  </div>
</template>
<style lang="css">
.bg-orange-sample {
  background-color: #e7541c;
}
.bg-blue-sample {
  background-color: #000099;
}
</style>
