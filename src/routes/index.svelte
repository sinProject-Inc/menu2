<script lang="ts">
  import header_image from '$lib/assets/images/images_photo_fu.jpg'
  import pork_katsu_image from '$lib/assets/images/a9426cb9-5950-4cde-a011-80672a2a7295.jpeg'
  import amoraisu from '$lib/assets/images/e75f8a24-7a68-4585-b4c5-2fc5763f7dfc.jpeg'

  import Item from '../lib/components/Item.svelte'
  import Shop from '../lib/components/Shop.svelte'
</script>

<div class="item_list">
  <Shop
    image_src={header_image}
    name="洋食の歩（エフ・ユー）"
    description="立ち飲み居酒屋・バー、弁当"
  />

  <Item
    image_src={amoraisu}
    name="アモライス"
    price="¥500"
    description="キャリア30年のホテルシェフが作るオムライス。 ご飯がチキンライスではなく当店オリジナルバターライスです。"
  />

  <Item
    image_src={pork_katsu_image}
    name="ポークカツ"
    price="¥500"
    description="揚げたてのポークカツをシャリアピンソースで"
  />
</div>

<style>
  :global(body) {
    margin: 0;
    font-size: 3.6vw;
  }

  .item_list {
    display: flex;
    flex-direction: column;
    gap: 4vw;
    background-color: #fafafa;
  }
</style>
