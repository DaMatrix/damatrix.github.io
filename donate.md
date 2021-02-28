---
layout: default
---

Want to support me and my projects? Consider donating via crypto (preferred) or PayPal. Thanks!


<div id="addresses">Loading...</div>

<script>
    fetch("https://gist.githubusercontent.com/DaMatrix/8b7ff92fcc7e49c0f511a8ed207d8e92/raw/www.daporkchop.net-donate-addresses.json").then(response => {
        return response.json();
    }).then(data => {
        var list = document.getElementById("addresses");
        list.innerHTML = "";
        for (let curr of data) {
            var span = document.createElement("span");
            
            var e = document.createElement("a");
            e.href = curr.url;
            e.innerText = curr.symbol;
            span.appendChild(e);
            
            e = document.createElement("span");
            e.innerText = ": ";
            span.appendChild(e);
            
            e = document.createElement("code");
            e.classList.add("highlighter-rouge");
            e.innerText = curr.address;
            span.appendChild(e);
            
            list.appendChild(span);
            list.appendChild(document.createElement("br"));
        }
    });
</script>

