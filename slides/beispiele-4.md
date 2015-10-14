#### Netflix Search
<pre><code class="javascript" data-trim>
let searchResultSets =
    return keyPresses
        .throttle(250)
        .map((key) => getJSON('/searchresults?q=' + input.value)
            .retry(3)
            .takeUntil(keyPresses)
        ).concatAll();

searchResultSets.forEach(
    (resultSet) => updateSearchResults(resultSet),
    (error) => showMessage('Server error!')
)
</code></pre>
