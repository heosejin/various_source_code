# various_source_code

### Counter-reset/Counter-increment(Reverse) - 일렬번호 매기기(역순)

style code
```html
    <style>
      .ex {
        counter-reset: cate 4;
      }
      .cate:after {
        counter-increment: cate -1;
        content: counter(cate, decimal-leading-zero) "";
      }
    </style>
```
    
html code
```html
      <article class="ex">
        <section>
          <p class="cate">project&nbsp;</p>
        </section>
        <section>
          <p class="cate">project</p>
        </section>
        <section>
          <p class="cate">project</p>
        </section>
      </article>
```
