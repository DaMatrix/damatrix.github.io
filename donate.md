---
layout: default
---

Want to support me and my projects? Consider donating via crypto (preferred) or PayPal. Thanks!

[![patreon badge](https://img.shields.io/badge/dynamic/json?color=e64413&label=Patreon&query=data.attributes.pledge_sum&prefix=$&suffix=/month&url=https%3A%2F%2Fwww.patreon.com%2Fapi%2Fcampaigns%2F727078)](https://www.patreon.com/DaPorkchop_)

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

