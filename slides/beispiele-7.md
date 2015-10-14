#### Push

<pre><code class="javascript" data-trim>
let source = getStockData();

source
  .filter((quote) => quote.price > 30)
  .map((quote) => quote.price)
  .forEach((price) => console.log('> $30: $' + price));
</code></pre>
