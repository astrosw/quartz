<!DOCTYPE html>
<html lang="en">
{{ partial "head.html" . }}

<body>
{{partial "search.html" .}}
<div id="index" class="singlePage">
    {{partial "header.html" .}}
    <img id="banner" src="https://thdngan.github.io/quartz/banner.svg" />
    <div class="bio">
       <div class="writing-sidebar">
            <div class="delay t-3">
	            <h2>My topics</h2>
	            <p>1. <a href="https://thdngan.github.io/quartz/subjects/climate">Climate</a></p>
	            <p>2. <a href="https://thdngan.github.io/quartz/subjects/image-processing">Image Processing</a></p>
	            <p>3. <a href="https://thdngan.github.io/quartz/subjects/particle-physics">Particle Physics</a></p>
	            <p>4. Projects</p>
	        </div>
	        <div class="delay t-4">
                <h2>Recent Posts</h2>
                {{$writing := where .Site.RegularPages "Section" "posts" }}
                <ul class="delay stagger">
                    {{range first 4 $writing }}
                    <li>
                        <div class="section">
                            <div class="desc">
                                <h3><a href="{{ .Permalink }}">{{- .Title -}}</a></h3>
                            </div>
                            <p class="meta">
                            {{.WordCount}} words on {{partial "date-fmt.html" .}} 
                            </p>
                            {{partial "tags.html" .}}
                        </div>
                    </li>
                    {{end}}
                </ul>
                <a href="/quartz/posts">See {{sub (len $writing) 3}} more →</a>
            </div>
    </div>
	    <article>
            <p><blockquote>One could say, in fact, that no story really has a beginning, and that no story really has an end, as all of the world's stories are as jumbled as the items in the arboretum, with their details and secrets all heaped together so that the whole story, from beginning to end, depends on how you look at it.</blockquote></p>
            <p class="delay t-2"> &mdash; Lemony Snicket, The End
            <div class="delay stagger">{{partial "textprocessing.html" . }}</div>
        </article>
</div>
<div class="delay t-5">
<hr/>
        {{partial "footerIndex.html" . }}
</div>
</body>
</html>