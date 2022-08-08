<!DOCTYPE html>
<html lang="en">
{{ partial "head.html" . }}

<body>
{{partial "search.html" .}}
{{partial "chat.html" .}}
<div id="index" class="singlePage">
    {{partial "header.html" .}}
    <img id="banner" src="/banner.svg" />
    <div class="bio">
        <div class="writing-sidebar">
            <div class="delay t-3">
                <article>
	                {{partial "toc.html" .}}
	                {{if $.Site.Data.config.enableRecentNotes}}
		                {{partial "recent.html" . }}
		            {{end}}
		        </article>
            </div>
        </div>
        <article>
            <p>Hello, I'm Ngân Trịnh. You can call me Ryan (I know "Ngân" might be hard to pronounce).</p>
            <div class="delay stagger">{{partial "textprocessing.html" . }}</div>
        </article>
    </div>
    <div class="delay t-4">
        {{partial "footerIndex.html" .}}
    </div>
</div>
</body>
</html>