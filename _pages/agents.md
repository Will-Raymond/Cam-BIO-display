---
title: ""
permalink: /equipment/
# Lab equipment. `agent` = id from _data/agents.yml; leave it off for
# equipment with no agent yet (it shows greyed out in the ecosystem map).
equipment:
  - name: "OpenTrons FLEX"
    agent: robert
    parts: ["Automated thermocycler", "Heater shaker", "96 head pipetter"]
  - name: "Automatic plate pourer"
  - name: "OpenTrons OT2 ×2 (\"Otto\")"
    agent: robert
  - name: "Dispendix I.DOT"
    agent: dotty
  - name: "Tapestation"
  - name: "PIXL colony picker"
  - name: "Eppendorf Epimotion 5705"
  - name: "Bambu H2C"
    agent: bambi
  - name: "Quantstudio"
---

# Meet our Agents

We are designing validated agents for our own machines, with tools for swappable LLM models. Click any agent in the map, or use the selector below, to see what it does.

{% include agents-explorer.html %}

<style>
  .manifest { margin: 2rem 0; border: 1px solid #dcdcdc; border-radius: 10px; background: #fff; }
  .manifest summary {
    cursor: pointer; list-style: none; display: flex; align-items: center; justify-content: space-between;
    padding: .9rem 1.25rem; font-size: 1.25rem; font-weight: 700; color: #0e2431;
  }
  .manifest summary::-webkit-details-marker { display: none; }
  .manifest summary::after { content: "+"; font-size: 1.5rem; line-height: 1; color: #7E5475; transition: transform .2s; }
  .manifest[open] summary::after { transform: rotate(45deg); }
  .manifest summary:hover, .manifest summary:focus-visible { color: #7E5475; outline: none; }
  .manifest summary small { font-size: .8rem; font-weight: 400; color: #6b7680; margin-left: .5rem; }
  .manifest ul { margin: 0; padding: 0 1.25rem 1rem 2.5rem; }
  .manifest li { margin: .3rem 0; }
  .manifest li em { color: #7E5475; }
</style>

<details class="manifest">
  <summary><span>Full equipment manifest<small>{{ page.equipment.size }} instruments</small></span></summary>
  <ul>
    {% for e in page.equipment %}
    <li>{{ e.name }}{% if e.agent %} — <em>{{ site.data.agents | where: "id", e.agent | map: "name" | first }}</em>{% endif %}
      {% if e.parts %}<ul>{% for p in e.parts %}<li>{{ p }}</li>{% endfor %}</ul>{% endif %}
    </li>
    {% endfor %}
  </ul>
</details>

[See our experiments →]({{ "/experiments/" | relative_url }})
{: .notice--info}
