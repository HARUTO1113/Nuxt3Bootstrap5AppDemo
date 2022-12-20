<template>
  <div class="container text-center my-5">
    <h1>{{ data.title }}</h1>
    <div class="alert alert-primary" role="alert">{{ data.description }}</div>
  </div>
  <div class="container mb-5">
    <div class="card mb-3 mx-auto">
      <div class="row g-0">
        <div class="col-md-4">
          <img
            src="https://img.cpcdn.com/recipes/3695776/894x1461s/03855e67f64548a05b1f995faabe8f57?u=12868943&p=1455726325"
            class="img-fluid rounded-start" alt="...">
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="card-title">{{data.zairyou}}</h5>
            <div class="card-text">
              <ul>
                <li v-for="item in data.material">{{ item.text }}</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="container mb-5">
    <h2>{{data.tukurikata}}</h2>
    <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4">
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">1</span></div>
        <ul>
                <li v-for="item in data.material">{{ item.text }}</li>
        </ul>
        <p>{{data.t1}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">2</span></div>
        <p>{{data.t2}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">3</span></div>
        <p>{{data.t3}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">4</span></div>
        <p>{{data.t4}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">5</span></div>
        <p>{{data.t5}}<br />
        {{data.t6}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">6</span></div>
        <p>{{data.t7}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">7</span></div>
        <p>{{data.t8}}<br />
          {{data.t9}}</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">8</span></div>
        <p>160度で5分以上、様子を見ながら、火が通ったら、一度上げて、今度は180～200度でカリっと仕上げ、完成です☆</p>
      </div>
      <div class="col border p-2">
        <div class="mb-2"><span class="badge bg-secondary">9</span></div>鶏肉の1枚はサイズにばらつきがある為、2～3枚という記載に変更しました。
      </div>
      </ul>
    </div>
    <ol>

    </ol>
  </div>
  <div class="container mb-5">
    <div class="row gx-5">
      <div class="col-sm">
        <h3>コツ・ポイント</h3>

        <p>揚げる際鍋底での焦げ防止に衣が軽く揚がるまで菜箸等で時々浮かせて下さい</p>
        <p>好みで粉類に粗びき黒胡椒小さじ1/2を足しても◎</p>
        <p>にんにくチューブ２センチはガーリックパウダー小さじ１に変えて粉類と混ぜても美味しいです。</p>
        <p>パプリカパウダーは無くても可</p>
      </div>
      <div class="col-sm">
        <h3>このレシピの生い立ち</h3>

        <p>今まで作ったKFCレシピは、卵液や粉もかなり余るし、何よりも
          何かひと味足りない……と思って、やっとKFC味にたどり着きました！</p>
        <p>どの家庭にもあるような材料で☆</p>
        <p>牛乳と卵液、粉類も必要量のみになっているので無駄が無く経済的です☆</p>
      </div>
    </div>
  </div>
</template>
<script setup>
const data = useRecipe()
</script>
