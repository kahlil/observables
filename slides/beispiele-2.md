#### Top Filme anzeigen

<pre><code class="javascript" data-trim>
let getTopRatedFilms = (user) => {
    return user.videoLists
        .map((videoList) => videoList.videos
            .filter((v) => v.rating === 5)
            // -> [[vids mit rating 5], [vids mit rating 5], ...]
        ).concatAll();
};

getTopRatedFilms(me)
    .forEach(displayMovie);
</code></pre>
