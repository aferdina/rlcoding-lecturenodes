# rlcoding-lecturenodes

## Usage

### Some useful commands

```sh
find . -type f \( -name "*.aux" -o -name "*.bbl" -o -name "*.blg" -o -name "*.log" -o -name "*.nav" -o -name "*.out" -o -name "*.snm" -o -name "*.toc" -o -name "*.vrb" -o -name "*.run.xml" -o -name "*.pdf" -o -name "*.fls" -o -name "*.gz" -o -name "*.loc" -o -name "*.soc" -o -name "*.fdb_latexmk" \) -delete
```

Download chatgpt output as Markdown:

```sh
function h(html) { return html.replace(/<p>/g, '\n\n').replace(/<\/p>/g, '').replace(/<b>/g, '**').replace(/<\/b>/g, '**').replace(/<i>/g, '_').replace(/<\/i>/g, '_').replace(/<code[^>]*>/g, (match) => { const lm = match.match(/class="[^"]*language-([^"]*)"/); return lm ? '\n```' + lm[1] + '\n' : '```'; }).replace(/<\/code[^>]*>/g, '```').replace(/<[^>]*>/g, '').replace(/Copy code/g, '').replace(/This content may violate our content policy. If you believe this to be in error, please submit your feedback — your input will aid our research in this area./g, '').trim(); } (()=>{ const e=document.querySelectorAll(".text-base");let t="";for(const s of e)s.querySelector(".whitespace-pre-wrap")&&(t += t == ""?"":"--------\n", t+=`**${s.querySelectorAll('img').length>1?s.querySelectorAll('img')[1].alt:'ChatGPT'}**: ${h(s.querySelector(".whitespace-pre-wrap").innerHTML)}\n\n`);const o=document.createElement("a");o.download=(document.querySelector(".pr-14.bg-gray-800")?.innerText||"Conversation with ChatGPT")+".md",o.href=URL.createObjectURL(new Blob([t])),o.style.display="none",document.body.appendChild(o),o.click()})();
```

### Icons from flaticon

<a href="https://www.flaticon.com/free-icons/target" title="target icons">Target icons created by srip - Flaticon</a>
