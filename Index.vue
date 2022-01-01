<template>
  <q-page class="flex flex-center">
    <div>
    <div>
    </div>
    <div>
    <form>
      <h4>Визуализация содержания текста об компьютерных играх</h4>
    <div>
    </div>
    </form>
    <div class="q-pa-md row items-start q-gutter-md">
    <q-card dark bordered class="bg-grey-9 my-card">
      <q-card-section>
        <div class="text-h6">Актуальность проекта</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        В настоящее время существует свыше 200000 игр на различные виды устройств, и каждый день выходят всё новые игры.

Однако в данный момент на рынке игр существует проблемы с выбором этих самых игр, которые бы удовлетворяли покупателя и игрока.

Наличие данных проблем наделяют данную программу конкурентными преимуществами.
      </q-card-section>
    </q-card>
    </div>
    <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card">
      <q-card-section>
        <div class="text-h6">Задачи и цель проекта.</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        Основная цель проекта – разработать программу для быстрого выяснения главных моментов компьютерных игр
Задача проекта:
	1) Изучить основы языка программирования Python;
	2) Написать код для корректной работы программы;
	3) Описать функционал разрабатываемого сервиса;
	4) Разработать прототип проекта и его алгоритмы;
	5) Определение перспектив развития.

      </q-card-section>
    </q-card>
    <div class="q-pa-md row items-start q-gutter-md">
    <q-card
      class="my-card text-white"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
    >
      <q-card-section>
        <div class="text-h6">Ключевые моменты исходного кода проекта</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        Программа: CGProgect
Язык программирования: Python
Среда разработки: Python 3.7
Платформа: PyCharm
Используемые алгоритмы: TextRank, RakeRank.

      </q-card-section>
    </q-card>
    </div>
    <div class="q-pa-md row items-start q-gutter-md">
    <q-card flat bordered class="my-card">
      <q-card-section>
        <div class="text-h6">Используемые фреймворки и библиотеки</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        Программное средство будет выглядеть в виде клиент-серверного приложения. Сервер будет написан на Python, использована библиотека Flask + дополнительные библиотеки текстовой аналитики.
      </q-card-section>
    </q-card>
    </div>
<div class="q-pa-md row items-start q-gutter-md">
    <q-card
      class="my-card text-white"
      style="background: radial-gradient(circle, #7CFC00 0%, #32CD32 100%)"
    >
      <q-card-section>
        <div class="text-h6">Перспективы развития проекта</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        1) Добавить графический интерфейс
        2) Добавить локализацию на английский язык
        3) Избавиться от возможных ошибок

      </q-card-section>
    </q-card>
    </div>
    </div>
    <div class="q-pa-md row items-start q-gutter-md">
    <q-card dark bordered class="bg-grey-9 my-card">
      <q-card-section>
        <div class="text-h6">Результаты проекта</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        В ходе работы была выполнена главная цель и задачи, поставленные ранее:
        - Изучены основы языка программирования Python и среды разработки;
        - Изучены основы создания принципиальных программ;
        - Описан функционал разрабатываемого сервиса;
        - Разработан прототип программы и ее алгоритмы

      </q-card-section>
    </q-card>
    </div>

    </div>
</div>
  </q-page>
</template>
<script>
import { defineComponent } from 'vue';
import { ref } from 'vue'
export default defineComponent({
  name: 'PageIndex',
    setup () {
    return {
      text: ref('')
    }
  },
  data() {
    return{
      title:"",
      body:"",
      posts:[
        {id: 1, title: 'Test Vue', body: 'Описание поста'},
        {id: 1, title: 'Test Vue', body: 'Описание поста'},
        {id: 1, title: 'Test Vue', body: 'Описание поста'},
      ]
    }
 
  },
 methods: {
    btn_click () {
      alert(this.text)
    },
    create_post(){
      const newPost= {
        id: Date.now(),
        title: this.title,
        body: this.body,
      }
      this.posts.push(newPost)
    }
  },
 
})
 
</script>
<style scoped>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
 
}
div{
 
display: flex;
flex-direction: column;
}
.post{
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
}
.input{
  width: 100%;
  border: 1px solid teal;
  padding: 10px 15px ;
  margin-top: 15px;
}
.btn{
  align-self: flex-end;}
</style>