---
layout: center
highlighter: shiki
css: unocss
colorSchema: dark
transition: fade-out
title: Gestão da Qualidade
lineNumbers: false
drawings:
  persist: false
mdc: true
clicks: 0
preload: false
glowSeed: 200
routerMode: hash
class: flex justify-center items-center gap-20 px-40 text-xl
addons:
  - tldraw
---

<div translate-x--35>

# Cultura e Liderança

Gestão da Qualidade

</div>

<style>
  h1 {
    font-weight: bold
  }
</style>

---
class: flex justify-center items-center gap-20 px-40 text-xl
clicks: 2
glowSeed: 203
---

<div
  absolute text-6xl
  :class="$clicks < 1 ? 'text-white' : 'translate-y--18 scale-40 text-white/30'"
  transition duration-500 ease-in-out
>
  <span transition="all 1000! ease-in-out" :class="$clicks > 1 ? 'opacity-0' : ''">🎭 Cultura da Liderança</span>
</div>

<div flex flex-col items-center>
  <v-clicks>
    <div mt-4 transition="all ease-in-out" flex items-center
      duration-1500 :class="$slidev.nav.clicks > 1 ? 'translate-x-[-260px] translate-y-[-218px]' : ''">
      <h1 flex items-center font-bold transition="all duration-1000 ease-in-out" :class="$slidev.nav.clicks > 1 ? 'text-3xl!' : 'text-5xl!'">
        <span>✳️ Principais Características</span>
      </h1>
    </div>
  </v-clicks>
</div>

---
glowSeed: 203
---

<div flex="row ~" w-full justify-between>
  <div>
    <div text-left w-full h-full flex="~ col justify-center">
      <div class="font-bold text-3xl mb-8">✳️ Principais Características</div>
        <div class="space-y-2 list-decimal pl-4">
          <div v-click>🎯 Foco no cliente interno e externo</div>
          <div v-click>📈 Compromisso com a melhoria contínua</div>
          <div v-click>✅ Valorização da padronização de processos</div>
          <div v-click>🎉 Incentivo à participação e envolvimento de todos os colaboradores</div>
          <div v-click>💬 Comunicação clara e transparente</div>
        </div>
      </div>
  </div>
</div>

---

<tldraw class="w-200 h-120" doc="tldraw/doc-rxc69jiEj2HVqUgTWJ-LF.json"></tldraw>

---
class: flex justify-center items-center gap-20 px40 text-xl overflow-hidden
clicks: 1
---

<div text-4xl absolute :class="$clicks < 1 ? 'text-white' : 'translate-y--18 scale-40 text-white/30'" transition duration-500 ease-in-out>
  <span>✨ Liderança</span>
</div>

<div flex flex-col items-center relative>
  <div
    mt-15
    :class="[
      $clicks === 0 ? 'opacity-0' : '',
      $clicks === 1 ? 'opacity-100' : '',
      $clicks > 1 ? 'opacity-30 blur-sm' : ''
    ]"
    transition duration-500
  >

  <h1 flex items-center text="5xl!">
    <span>📑 Papéis da Liderança</span>
  </h1>

  </div>
</div>

---
glowSeed: 203
---

<div flex="row ~" w-full justify-between>
  <div>
    <div text-left w-full h-full flex="~ col justify-center">
      <div class="font-bold text-3xl mb-8">📑 Papéis da Liderança</div>
        <div class="space-y-2 list-decimal pl-4">
          <div v-click>🎯 Definir uma visão clara para a qualidade, alinhada à missão e valores da organização</div>
          <div v-click>🌟 Servir como exemplo de comprometimento e responsabilidade</div>
          <div v-click>🤝 Promover um ambiente de confiança, abertura e cooperação</div>
          <div v-click>🧠 Incentivar a capacitação e o desenvolvimento de competências</div>
          <div v-click>🥳 Reconhecer e valorizar conquistas relacionadas à qualidade</div>
        </div>
      </div>
  </div>
</div>

---
class: py-10
clicks: 6
glowSeed: 350
---

# Integração e Benefícios

<span>Cultura da Qualidade e Liderança</span>

<div mt-6 />

<div grid grid-cols-2 gap-6>
  <div
    v-click="1"
    border="2 solid blue-800" bg="blue-800/20"
    rounded-lg overflow-hidden
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 translate-y-20' : 'opacity-100 translate-y-0'"
  >
    <div bg="blue-800/40" px-4 py-2 flex items-center>
      <span font-bold>⚙️ Integração</span>
    </div>
    <div px-5 py-3>
      <div
        v-for="(step, idx) in [
          'Programas de treinamento e capacitação contínua',
          'Estabelecimento de indicadores de desempenho',
          'Monitoramento de resultados',
          'Promoção de um ambiente de inovação e aprendizagem',
          'Reconhecimento de boas práticas que contribuam para a qualidade'
        ]"
        :key="step"
        flex items-center gap-2 py-1
        :class="$clicks < 1 ? 'opacity-0' : 'opacity-100'"
        :style="{ transitionDelay: `${200 + idx * 100}ms`, transitionProperty: 'all', transitionDuration: '500ms' }"
      >
        🔵
        <span>{{step}}</span>
      </div>
    </div>
  </div>

  <div
    v-click="2"
    border="2 solid lime-800" bg="lime-800/20"
    rounded-lg overflow-hidden
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div bg="lime-800/40" px-4 py-2 flex items-center>
      <span font-bold>🎊 Benefícios</span>
    </div>
    <div px-5 py-4 flex flex-col gap-2>
      <div
        v-for="(item, idx) in [
          'Maior satisfação e fidelização de clientes',
          'Redução de custos com retrabalho e desperdícios',
          'Aumento da produtividade e da eficiência dos processos',
          'Fortalecimento da imagem institucional',
          'Engajamento e motivação dos colaboradores'
        ]"
        :key="item"
        v-click="2 + idx"
        flex items-center gap-2
        :class="$clicks < (2 + idx) ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
        transition duration-300 ease-in-out
      >
        ✅
        <span>{{item}}</span>
      </div>
    </div>
  </div>
</div>

<style>
  h1 {
    font-weight: bold
  }
</style>

---
layout: intro
class: px-24
glowSeed: 205
---

<div flex items-center justify-center>
  <div
    v-click flex flex-col gap-2 items-center justify-center transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'translate-x--20' : 'translate-x-0'"
  >
    <div font-bold text-3xl text-center>
      📚
      <br>
      Gestão da Qualidade
    </div>
  </div>
  <div
    v-after pl-15 pr-15 transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'scale-80' : 'scale-100'"
  >
    <div i-carbon:close text-8xl />
  </div>
  <div
    v-after flex flex-col gap-2 items-center justify-center transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'translate-x-20' : 'translate-x-0'"
  >
    <div font-bold text-3xl text-center>
      🖥️
      <br>
      Desenvolvimento <br> de Software
    </div>
  </div>
</div>

---
class: py-10
glowSeed: 100
---

# Principais Objetivos

<span>Qualidade no Desenvolvimento de Software</span>

<div mt-4 />

<div flex flex-col gap-3>

<v-clicks>

<div border="2 solid blue-800/50" rounded-lg>
  <div flex items-center text-base bg="blue-800/30" px-3 py-2 text-blue-300>
    🤗&nbsp;<em>Satisfação do Cliente</em>
  </div>
  <div bg="blue-800/10" px-4 py-3>
    <div>
      <span>
        Entregar um software que atenda as expectativas do usuário final.
      </span>
    </div>
  </div>
</div>

<div border="2 solid teal-800/50" rounded-lg>
  <div flex items-center text-base bg="teal-800/30" px-3 py-2 text-teal-300>
    💸&nbsp;<em>Redução de Custos</em>
  </div>
  <div bg="teal-800/10" px-4 py-3>
    <div>
      <span>
        Identificar e corrigir bugs no início, evitando mais trabalho e custos futuramente.
      </span>
    </div>
  </div>
</div>

<div border="2 solid cyan-800/50" rounded-lg>
  <div flex items-center text-base bg="cyan-800/30" px-3 py-2 text-cyan-300>
     📈&nbsp;<em>Aumento da Confiabilidade</em>
  </div>
  <div bg="cyan-800/10" px-4 py-3>
    <div>
      <span>
        Garantir que o software opere de forma consistente e sem falhas, mesmo sob condições diversas.
      </span>
    </div>
  </div>
</div>

<div border="2 solid rose-800/50" rounded-lg>
  <div flex items-center text-base bg="rose-800/30" px-3 py-2 text-rose-300>
      ⚖️&nbsp;<em>Conformidade Regulatória</em>
  </div>
  <div bg="rose-800/10" px-4 py-3>
    <div>
      <span>
        Atender a normas e regulamentações específicas do setor.
      </span>
    </div>
  </div>
</div>

</v-clicks>

</div>

<style>
  h1 {
    font-weight: bold
  }
</style>

---
class: flex justify-center items-center gap-20 px-40 text-xl
clicks: 14
glowSeed: 203
---

<div
  absolute text-6xl
  :class="$clicks < 1 ? 'text-white' : 'translate-y--18 scale-40 text-white/30'"
  transition duration-500 ease-in-out
>
  <span transition="all 1000! ease-in-out" :class="$clicks > 1 ? 'opacity-0' : ''">🤔 Como atingir os objetivos?</span>
</div>

<div flex flex-col items-center>
  <v-clicks>
    <div transition="all duration-1000 ease-in-out" :class="$slidev.nav.clicks > 0 ? 'opacity-100' : 'opacity-0'">
      <div mt-4 transition="all ease-in-out" flex flex-col flex-start
        duration-1500 :class="$slidev.nav.clicks > 1 ? 'translate-x-[-280px] translate-y-[-218px]' : ''">
        <h1 flex items-center font-bold transition="all duration-1000 ease-in-out" :class="$slidev.nav.clicks > 1 ? 'text-3xl! mb-3!' : 'text-5xl!'">
          <span>🏛️ Pilares Fundamentais</span>
        </h1>
        <span text-sm transition="all ease-in-out" :class="$slidev.nav.clicks > 1 ? 'opacity-50' : 'opacity-0'">Gestão da Qualidade no Desenvolvimento de Software</span>
      </div>
    </div>
  </v-clicks>
</div>

<div grid grid-cols-2 gap-4 absolute>
  <v-clicks>
    <div
      :class="$clicks < 3 ? 'opacity-0' : 'opacity-100'"
      rounded-lg
      border="2 solid blue-800/30" bg="blue-900/30"
      shadow-lg
      transition duration-500 ease-in-out
      flex
      h-12
    >
      <div px-2 py-2 flex items-center justify-center>
        📑
      </div>
      <div bg="blue-800/30" w-full px-3 py-2 flex items-center justify-center text-center font-bold>
        <span>Requisitos</span>
      </div>
    </div>
    <div
      :class="$clicks < 6 ? 'opacity-0' : 'opacity-100'"
      rounded-lg
      border="2 solid emerald-800/30" bg="emerald-900/30"
      shadow-lg
      transition duration-500 ease-in-out
      flex
      h-12
    >
      <div px-2 py-2 flex items-center justify-center>
        ⚙️
      </div>
      <div bg="emerald-800/30" w-full px-3 py-2 flex items-center justify-center text-center font-bold>
        <span>Processos</span>
      </div>
    </div>
    <div
      :class="$clicks < 9 ? 'opacity-0' : 'opacity-100'"
      rounded-lg
      border="2 solid orange-500/60" bg="orange-600/60"
      shadow-lg
      transition duration-500 ease-in-out
      flex
      h-12
    >
      <div px-2 py-2 flex items-center justify-center>
        🧪
      </div>
      <div bg="orange-500/60" w-full px-3 py-2 flex items-center justify-center text-center font-bold>
        <span>Testes</span>
      </div>
    </div>
    <div
      :class="$clicks < 12 ? 'opacity-0' : 'opacity-100'"
      rounded-lg
      border="2 solid rose-600/30" bg="rose-700/40"
      shadow-lg
      transition duration-500 ease-in-out
      flex
      h-12
    >
      <div px-2 py-2 flex items-center justify-center>
        📈
      </div>
      <div bg="rose-600/30" w-full px-3 py-2 flex items-center justify-center text-center font-bold>
        <span>Melhoria Contínua</span>
      </div>
    </div>
  </v-clicks>
</div>

<div
  absolute
  class="inset-0 flex items-center justify-center"
  :class="$clicks === 4 ? 'backdrop-blur-md bg-black/30' : 'opacity-0 translate-y-0 scale-90'"
  transition duration-800 ease-in-out
  v-click
>
  <div border="2 solid blue-600" bg="blue-800/40" rounded-lg w="[50%]">

  <div font-bold rounded-t-lg bg="blue-800" px-4 py-3>Definição de Requisitos Claros</div>

  <div px-4 py-3 text-sm>
    A qualidade começa na fase de levantamento de requisitos. Requisitos ambíguos ou incompletos são uma das maiores causas de problemas.
  </div>

  </div>
</div>

<div
  absolute
  class="inset-0 flex items-center justify-center"
  :class="$clicks === 7 ? 'backdrop-blur-md bg-black/30' : 'opacity-0 translate-y-0 scale-90'"
  transition duration-800 ease-in-out
  v-click
>
  <div border="2 solid emerald-600" bg="emerald-800/40" rounded-lg w="[50%]">

  <div font-bold rounded-t-lg bg="emerald-800" px-4 py-3>Processos de Desenvolvimento Bem Definidos</div>

  <div px-4 py-3 text-sm>
    A adoção de metodologias (como Scrum, Kanban ou outras dependendo do contexto) e a padronização de processos são essenciais para a consistência.
  </div>

  </div>
</div>

<div
  absolute
  class="inset-0 flex items-center justify-center"
  :class="$clicks === 10 ? 'backdrop-blur-md bg-black/30' : 'opacity-0 translate-y-0 scale-90'"
  transition duration-800 ease-in-out
  v-click
>
  <div border="2 solid orange-300" bg="orange-500/60" rounded-lg w="[50%]">

  <div font-bold rounded-t-lg bg="orange-500" px-4 py-3>Testes</div>

  <div px-4 py-3 text-sm>
     A fase de testes é crítica e envolve diversos tipos, como testes de unidade, integração, sistema, aceitação, performance, segurança e usabilidade. Automação de testes é um facilitador poderoso.
  </div>

  </div>
</div>

<div
  absolute
  class="inset-0 flex items-center justify-center"
  :class="$clicks === 13 ? 'backdrop-blur-md bg-black/30' : 'opacity-0 translate-y-0 scale-90'"
  transition duration-800 ease-in-out
  v-click
>
  <div border="2 solid rose-600" bg="rose-800/80" rounded-lg w="[50%]">

  <div font-bold rounded-t-lg bg="rose-800" px-4 py-3>Melhoria Contínua</div>

  <div px-4 py-3 text-sm>
    A cultura de feedback e aprendizado é essencial. Após cada ciclo de desenvolvimento, as equipes devem analisar o que funcionou e o que pode ser aprimorado.
  </div>

  </div>
</div>

---
class: flex justify-center items-center gap-20 px-40 text-xl
glowSeed: 203
---

<div flex flex-col items-center>
    <div mt-4 transition="all ease-in-out" text-center duration-1500>
      <h1 flex items-center font-bold text-4xl transition="all duration-1000 ease-in-out">
       💯 <br> Métricas para um <br> Software de Qualidade
      </h1>
    </div>
</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Confiabilidade</span>

<div mt-16 />

<div>

  <div class="flex flex-col justify-center items-center">
    <div v-click="1" class="rounded-lg p-8 bg-teal-900/20 text-center flex flex-col justify-center items-center gap-2">
      <svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="#009689" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-shield-check-icon lucide-shield-check"><path d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"/><path d="m9 12 2 2 4-4"/></svg>
      <div font-bold text-sm text-nowrap mt-2>Confiabilidade</div>
    </div>
  </div>

  <div v-click="2">
    <div text-center class="mt-6">
      Capacidade do sistema de funcionar de forma <span v-mark="{ at: 3, color: 'rgb(144, 200, 255)', type: 'underline' }">consistente</span> e sem falhas <span v-mark="{ at: 4, color: 'rgb(144, 200, 255)', type: 'underline' }">inesperadas.</span>
    </div>
  </div>

</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Confiabilidade</span>

<div mt-8 />

<div v-click="1" class="bg-teal-900/20 rounded-lg p-4">
  <div font-bold text-teal-300 mb-2 flex items-center>
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-copy-check-icon lucide-copy-check"><path d="m12 15 2 2 4-4"/><rect width="14" height="14" x="8" y="8" rx="2" ry="2"/><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"/></svg>
    <span class="mt-1 ml-2">Aplicação Prática</span>
  </div>
  <div class="text-xs bg-teal-800/30 rounded p-2 font-mono">
    Um sistema que não trava durante uma transação ou em operações em tempo real.
  </div>
</div>

<div v-click="2" class="mt-4 border-2 border-emerald-500/30 rounded-lg p-2 bg-emerald-900/20">
  <div text-xl font-bold mb-4 text-emerald-300 flex items-center>
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-spotlight-icon lucide-spotlight"><path d="M15.295 19.562 16 22"/><path d="m17 16 3.758 2.098"/><path d="m19 12.5 3.026-.598"/><path d="M7.61 6.3a3 3 0 0 0-3.92 1.3l-1.38 2.79a3 3 0 0 0 1.3 3.91l6.89 3.597a1 1 0 0 0 1.342-.447l3.106-6.211a1 1 0 0 0-.447-1.341z"/><path d="M8 9V2"/></svg>
    <span class="mt-1 ml-2">Exemplos</span>
  </div>
  <div space-y-3>
    <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
      <div font-bold>WhatsApp</div>
      <div text-xs text-emerald-200>Mensagens entregues em tempo real</div>
    </div>
    <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
      <div font-bold>PayPal</div>
      <div text-xs text-emerald-200>Confiável em transações financeiras</div>
    </div>
    <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
      <div font-bold>Caixa Eletrônico</div>
      <div text-xs text-emerald-200>Alta estabilidade em operações</div>
    </div>
  </div>
</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Escalabilidade</span>

<div mt-16 />

<div>

  <div class="flex flex-col justify-center items-center">
    <div v-click="1" class="rounded-lg p-8 bg-teal-900/20 text-center flex flex-col justify-center items-center gap-2">
      <svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="#009689" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chart-no-axes-combined-icon lucide-chart-no-axes-combined"><path d="M12 16v5"/><path d="M16 14v7"/><path d="M20 10v11"/><path d="m22 3-8.646 8.646a.5.5 0 0 1-.708 0L9.354 8.354a.5.5 0 0 0-.707 0L2 15"/><path d="M4 18v3"/><path d="M8 14v7"/></svg>
      <div font-bold text-sm text-nowrap mt-2>Escalabilidade</div>
    </div>
  </div>

  <div v-click="2">
    <div text-center class="mt-6">
      Capacidade de  <span v-mark="{ at: 3, color: 'rgb(144, 200, 255)', type: 'underline' }">crescer</span> em número de usuários e dados <span v-mark="{ at: 4, color: 'rgb(144, 200, 255)', type: 'underline' }">sem comprometer</span>o desempenho.
    </div>
  </div>

</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Escalabilidade</span>

<div mt-8 />

<div v-click="1" class="bg-teal-900/20 rounded-lg p-4">
  <div font-bold text-teal-300 mb-2 flex items-center>
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-copy-check-icon lucide-copy-check"><path d="m12 15 2 2 4-4"/><rect width="14" height="14" x="8" y="8" rx="2" ry="2"/><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"/></svg>
    <span class="mt-1 ml-2">Aplicação Prática</span>
  </div>
  <div class="text-xs bg-teal-800/30 rounded p-2 font-mono">
    Uma rede social que suporta milhões de acessos simultâneos.
  </div>
</div>

<div class="flex gap-4 mt-4">
  <div v-click="2" class="basis-2/3 border-2 border-emerald-500/30 rounded-lg p-2 bg-emerald-900/20">
    <div text-xl font-bold mb-4 text-emerald-300 flex items-center>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-spotlight-icon lucide-spotlight"><path d="M15.295 19.562 16 22"/><path d="m17 16 3.758 2.098"/><path d="m19 12.5 3.026-.598"/><path d="M7.61 6.3a3 3 0 0 0-3.92 1.3l-1.38 2.79a3 3 0 0 0 1.3 3.91l6.89 3.597a1 1 0 0 0 1.342-.447l3.106-6.211a1 1 0 0 0-.447-1.341z"/><path d="M8 9V2"/></svg>
      <span class="mt-1 ml-2">Exemplos</span>
    </div>
    <div space-y-3>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>WhatsApp</div>
        <div text-xs text-emerald-200>Mensagens entregues em tempo real</div>
      </div>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>PayPal</div>
        <div text-xs text-emerald-200>Confiável em transações financeiras</div>
      </div>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>Caixa Eletrônico</div>
        <div text-xs text-emerald-200>Alta estabilidade em operações</div>
      </div>
    </div>
  </div>

  <div v-click="3" class="basis-1/3 border-2 border-rose-500/30 rounded-lg p-2 bg-rose-900/20">
    <div text-xl font-bold mb-4 text-rose-300 flex items-center>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-triangle-alert-icon lucide-triangle-alert"><path d="m21.73 18-8-14a2 2 0 0 0-3.48 0l-8 14A2 2 0 0 0 4 21h16a2 2 0 0 0 1.73-3"/><path d="M12 9v4"/><path d="M12 17h.01"/></svg>
      <span class="mt-1 ml-2">Fila Virtual</span>
    </div>
    <div space-y-3>
      <div class="px-4 py-2 bg-rose-800/30 rounded-lg text-sm">
        <div font-bold>Caixa Econômica</div>
      </div>
      <div class="px-4 py-2 bg-rose-800/30 rounded-lg text-sm">
        <div font-bold>Sites de venda de ingressos</div>
      </div>
      <div class="px-4 py-2 bg-rose-800/30 rounded-lg text-sm">
        <div font-bold>Black Friday</div>
      </div>
    </div>
  </div>
</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>UI/UX</span>

<div mt-16 />

<div>

  <div class="flex flex-col justify-center items-center">
    <div v-click="1" class="rounded-lg p-8 bg-teal-900/20 text-center flex flex-col justify-center items-center gap-2">
      <svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="#009689" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-pen-tool-icon lucide-pen-tool"><path d="M15.707 21.293a1 1 0 0 1-1.414 0l-1.586-1.586a1 1 0 0 1 0-1.414l5.586-5.586a1 1 0 0 1 1.414 0l1.586 1.586a1 1 0 0 1 0 1.414z"/><path d="m18 13-1.375-6.874a1 1 0 0 0-.746-.776L3.235 2.028a1 1 0 0 0-1.207 1.207L5.35 15.879a1 1 0 0 0 .776.746L13 18"/><path d="m2.3 2.3 7.286 7.286"/><circle cx="11" cy="11" r="2"/></svg>
      <div font-bold text-sm text-nowrap mt-2>UI/UX</div>
    </div>
  </div>

  <div v-click="2">
    <div text-center class="mt-6">
      <span v-mark="{ at: 3, color: 'rgb(144, 200, 255)', type: 'underline' }">Facilidade de uso</span> e <span v-mark="{ at: 4, color: 'rgb(144, 200, 255)', type: 'underline' }">experiência</span> agradável para o usuário.
    </div>
  </div>

</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>UI/UX</span>

<div mt-24 />

<div v-click="1" class="bg-teal-900/20 rounded-lg p-4">
  <div font-bold text-teal-300 mb-2 flex items-center>
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-copy-check-icon lucide-copy-check"><path d="m12 15 2 2 4-4"/><rect width="14" height="14" x="8" y="8" rx="2" ry="2"/><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"/></svg>
    <span class="mt-1 ml-2">Aplicação Prática</span>
  </div>
  <div class="text-xs bg-teal-800/30 rounded p-2 font-mono">
    Sistemas com interfaces simples e intuitivas que cumprem o objetivo.
  </div>
</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>UI/UX</span>

<div mt-8 />

<div class="flex gap-6">

  <div v-click="1" class="basis-1/2 border-2 border-emerald-500/30 rounded-lg p-2 bg-emerald-900/20">
    <div text-xl font-bold mb-4 text-emerald-300 flex items-center>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-spotlight-icon lucide-spotlight"><path d="M15.295 19.562 16 22"/><path d="m17 16 3.758 2.098"/><path d="m19 12.5 3.026-.598"/><path d="M7.61 6.3a3 3 0 0 0-3.92 1.3l-1.38 2.79a3 3 0 0 0 1.3 3.91l6.89 3.597a1 1 0 0 0 1.342-.447l3.106-6.211a1 1 0 0 0-.447-1.341z"/><path d="M8 9V2"/></svg>
      <span class="mt-1 ml-2">Exemplos</span>
    </div>
    <div space-y-3>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>Amazon</div>
        <div text-xs text-emerald-200>Compras em poucos cliques</div>
      </div>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>Airbnb</div>
        <div text-xs text-emerald-200>Design intuitivo para reservas</div>
      </div>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>Duolingo</div>
        <div text-xs text-emerald-200>Gamificação para aprendizado de idiomas</div>
      </div>
    </div>
  </div>

  <div v-click="2" class="basis-1/2">
    <n-carousel arrow draggable class="carousel">
      <img
        class="carousel-img"
        src="/amazon.jpg"
      >
      <img
        class="carousel-img"
        src="/airbnb.jpg"
      >
      <img
        class="carousel-img"
         src="/duolingo.png"
      >
    </n-carousel>
  </div>

  <style scoped>
    .carousel-img {
      width: 100%;
      height: 240px;
      object-fit: fill;
    }
  </style>

</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Performance</span>

<div mt-16 />

<div>

  <div class="flex flex-col justify-center items-center">
    <div v-click="1" class="rounded-lg p-8 bg-teal-900/20 text-center flex flex-col justify-center items-center gap-2">
      <svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="#009689" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-zap-icon lucide-zap"><path d="M4 14a1 1 0 0 1-.78-1.63l9.9-10.2a.5.5 0 0 1 .86.46l-1.92 6.02A1 1 0 0 0 13 10h7a1 1 0 0 1 .78 1.63l-9.9 10.2a.5.5 0 0 1-.86-.46l1.92-6.02A1 1 0 0 0 11 14z"/></svg>
      <div font-bold text-sm text-nowrap mt-2>Performance</div>
    </div>
  </div>

  <div v-click="2">
    <div text-center class="mt-6">
      <span v-mark="{ at: 3, color: 'rgb(144, 200, 255)', type: 'underline' }">Velocidade</span> e <span v-mark="{ at: 4, color: 'rgb(144, 200, 255)', type: 'underline' }">eficiência</span> com que o software executa suas funções.
    </div>
  </div>

</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Performance</span>

<div mt-24 />

<div v-click="1" class="bg-teal-900/20 rounded-lg p-4">
  <div font-bold text-teal-300 mb-2 flex items-center>
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-copy-check-icon lucide-copy-check"><path d="m12 15 2 2 4-4"/><rect width="14" height="14" x="8" y="8" rx="2" ry="2"/><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"/></svg>
    <span class="mt-1 ml-2">Aplicação Prática</span>
  </div>
  <div class="text-xs bg-teal-800/30 rounded p-2 font-mono">
    Sistemas capazes de carregar páginas em menos de 2 segundos.
  </div>
</div>

---
class: py-10
glow: bottom
glowSeed: 368
---

# 💯 Métricas

<span>Performance</span>

<div mt-8 />

<div class="flex gap-6">

  <div v-click="1" class="basis-1/2 border-2 border-emerald-500/30 rounded-lg p-2 bg-emerald-900/20">
    <div text-xl font-bold mb-4 text-emerald-300 flex items-center>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-spotlight-icon lucide-spotlight"><path d="M15.295 19.562 16 22"/><path d="m17 16 3.758 2.098"/><path d="m19 12.5 3.026-.598"/><path d="M7.61 6.3a3 3 0 0 0-3.92 1.3l-1.38 2.79a3 3 0 0 0 1.3 3.91l6.89 3.597a1 1 0 0 0 1.342-.447l3.106-6.211a1 1 0 0 0-.447-1.341z"/><path d="M8 9V2"/></svg>
      <span class="mt-1 ml-2">Exemplos</span>
    </div>
    <div space-y-3>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>McMaster-Carr</div>
        <div text-xs text-emerald-200>Ecommerce de alta performance</div>
      </div>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>Netflix</div>
        <div text-xs text-emerald-200>Streaming sem travar mesmo em HD/4K</div>
      </div>
      <div class="px-4 py-2 bg-emerald-800/30 rounded-lg text-sm">
        <div font-bold>Google Search</div>
        <div text-xs text-emerald-200>Resultados em milissegundos</div>
      </div>
    </div>
  </div>

  <div v-click="2" class="basis-1/2">
    <n-carousel arrow draggable class="carousel">
      <img
        class="carousel-img"
        src="/mcmaster-carr.jpg"
      >
      <img
        class="carousel-img"
        src="/netflix.jpg"
      >
      <img
        class="carousel-img"
         src="/google.jpg"
      >
    </n-carousel>
  </div>

  <style scoped>
    .carousel-img {
      width: 100%;
      height: 240px;
      object-fit: fill;
    }
  </style>

</div>
