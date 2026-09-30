<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0d1117,50:0b3d2e,100:00F5A0&height=280&section=header&text=Sani%20Shil&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20Developer%20%C2%B7%20Spring%20Boot%20%C2%B7%20Laravel&descSize=20&descAlignY=60" width="100%"/>

<a href="https://github.com/sanishil">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=900&color=00F5A0&center=true&vCenter=true&width=700&height=45&lines=Building+REST+APIs+that+scale;Spring+Boot+%C2%B7+Laravel+%C2%B7+Redis+%C2%B7+MySQL;Learning+System+Design+every+day" alt="Typing SVG"/>
</a>

<br/>

<img src="https://img.shields.io/badge/Spring_Boot-0d1117?style=flat-square&logo=springboot&logoColor=6DB33F"/>
<img src="https://img.shields.io/badge/Laravel-0d1117?style=flat-square&logo=laravel&logoColor=FF2D20"/>
<img src="https://img.shields.io/badge/Redis-0d1117?style=flat-square&logo=redis&logoColor=DC382D"/>
<img src="https://img.shields.io/badge/MySQL-0d1117?style=flat-square&logo=mysql&logoColor=4479A1"/>
<img src="https://img.shields.io/badge/Linux-0d1117?style=flat-square&logo=linux&logoColor=FCC624"/>

<br/>

<img src="https://komarev.com/ghpvc/?username=sanishil&label=Views&color=00f5a0&style=flat-square&labelColor=0d1117"/>
<img src="https://img.shields.io/github/followers/sanishil?style=flat-square&logo=github&color=00f5a0&labelColor=0d1117"/>
<img src="https://img.shields.io/github/stars/sanishil?style=flat-square&logo=github&color=00f5a0&labelColor=0d1117"/>

</div>

<br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=12,20&height=1&section=header" width="100%"/>

## `~/about`

```yaml
name:    Sani Shil
role:    Associate Software Development Engineer
main:    Java + Spring Boot
also:    Laravel / PHP
focus:   REST APIs · Caching · System Design
stack:   Redis · MySQL · Linux · Git
status:  Open to collaboration
mood:    Code • Build • Learn • Repeat
```

## `~/stack`

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,php,laravel,python,cpp,mysql,redis,angular,html,css,bootstrap,git,github,linux,postman&theme=dark&perline=8" />

</div>

## `~/skills`

<table width="100%">
<tr>
<th width="25%" align="left">☕ Spring Boot <i>(primary)</i></th>
<th width="25%" align="left">🐘 Laravel</th>
<th width="25%" align="left">⚡ Redis</th>
<th width="25%" align="left">🗄️ MySQL</th>
</tr>
<tr><td>REST APIs</td><td>REST APIs</td><td>Caching</td><td>Persistence</td></tr>
<tr><td>Spring Data JPA</td><td>MVC + Eloquent</td><td>Session storage</td><td>Spring integration</td></tr>
<tr><td>Validation &amp; exceptions</td><td>Middleware</td><td>Key-value access</td><td>Laravel integration</td></tr>
<tr><td>Auth &amp; authorization</td><td>Authentication</td><td>Reducing DB load</td><td>Query &amp; schema design</td></tr>
</table>

## `~/architecture`

<sub>How each stack in my toolbox flows, end to end.</sub>

### ☕ Spring Boot

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#0d1117','primaryTextColor':'#ffffff','primaryBorderColor':'#00F5A0','lineColor':'#00F5A0','secondaryColor':'#161b22','tertiaryColor':'#0d1117','fontFamily':'monospace'}}}%%
flowchart LR
    C(["Client"]) --> F["Security Filter<br/>JWT / Auth"]
    F --> CT["Controller<br/>RestController"]
    CT --> V{{"Validation<br/>Valid"}}
    V --> S["Service<br/>Business Logic"]
    S --> R["Repository<br/>Spring Data JPA"]
    R --> DB[("MySQL")]
    S -.-> RD[("Redis Cache")]
    CT -.-> EX["Global Exception<br/>Handler"]
    classDef spring stroke:#6DB33F,stroke-width:2px
    classDef data stroke:#4479A1,stroke-width:2px
    class F,CT,V,S,R,EX spring
    class DB,RD data
```

### 🐘 Laravel

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#0d1117','primaryTextColor':'#ffffff','primaryBorderColor':'#00F5A0','lineColor':'#00F5A0','secondaryColor':'#161b22','tertiaryColor':'#0d1117','fontFamily':'monospace'}}}%%
flowchart LR
    C(["Client"]) --> RT["Routes<br/>api.php / web.php"]
    RT --> MW["Middleware<br/>Auth / Throttle"]
    MW --> FR{{"Form Request<br/>Validation"}}
    FR --> CT["Controller"]
    CT --> M["Eloquent Model"]
    M --> DB[("MySQL")]
    CT -.-> RD[("Redis<br/>Cache / Session / Queue")]
    CT --> RES["API Resource<br/>JSON Response"]
    classDef lv stroke:#FF2D20,stroke-width:2px
    classDef data stroke:#4479A1,stroke-width:2px
    class RT,MW,FR,CT,M,RES lv
    class DB,RD data
```

### 🅰️ Angular

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#0d1117','primaryTextColor':'#ffffff','primaryBorderColor':'#00F5A0','lineColor':'#00F5A0','secondaryColor':'#161b22','tertiaryColor':'#0d1117','fontFamily':'monospace'}}}%%
flowchart LR
    U(["User"]) --> CMP["Component<br/>Template + Logic"]
    RTR["Router<br/>+ Guards"] --> CMP
    CMP --> SVC["Service<br/>Injectable"]
    SVC --> HC["HttpClient<br/>+ Interceptors"]
    HC --> API(["REST API"])
    API --> HC
    SVC -.-> RX["RxJS<br/>Observables"]
    RX -.-> CMP
    classDef ng stroke:#DD0031,stroke-width:2px
    class CMP,RTR,SVC,HC,RX ng
```

### 🐘 PHP

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#0d1117','primaryTextColor':'#ffffff','primaryBorderColor':'#00F5A0','lineColor':'#00F5A0','secondaryColor':'#161b22','tertiaryColor':'#0d1117','fontFamily':'monospace'}}}%%
flowchart LR
    C(["Browser"]) --> W["Web Server<br/>Apache / Nginx"]
    W --> I["index.php<br/>Front Controller"]
    I --> RT["Router"]
    RT --> CT["Controller"]
    CT --> M["Model<br/>PDO / MySQLi"]
    M --> DB[("MySQL")]
    CT --> VW["View / JSON"]
    VW --> C
    classDef php stroke:#777BB4,stroke-width:2px
    classDef data stroke:#4479A1,stroke-width:2px
    class W,I,RT,CT,M,VW php
    class DB data
```

### 🐍 Python

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#0d1117','primaryTextColor':'#ffffff','primaryBorderColor':'#00F5A0','lineColor':'#00F5A0','secondaryColor':'#161b22','tertiaryColor':'#0d1117','fontFamily':'monospace'}}}%%
flowchart LR
    IN(["Input<br/>Files / API / CLI"]) --> MAIN["Main Script"]
    MAIN --> MOD["Modules<br/>Functions / Classes"]
    MOD --> LIB["Libraries<br/>requests / pandas"]
    LIB --> PR["Processing<br/>Logic / Automation"]
    PR --> OUT(["Output<br/>Report / DB / Console"])
    classDef py stroke:#3776AB,stroke-width:2px
    class MAIN,MOD,LIB,PR py
```

## `~/stats`

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=sanishil&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&bg_color=0d1117&title_color=00F5A0&icon_color=00F5A0"/>
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sanishil&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00F5A0"/>

<img src="https://streak-stats.demolab.com?user=sanishil&theme=tokyonight&hide_border=true&background=0d1117&ring=00F5A0&fire=00F5A0&currStreakLabel=00F5A0"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=sanishil&theme=react-dark&hide_border=true&area=true&color=00F5A0&line=00F5A0&point=ffffff&bg_color=0d1117" width="100%"/>

</div>

## `~/now`

```diff
+ Building & improving REST APIs with Spring Boot and Laravel
+ Optimising performance with Redis caching
+ Deep-diving into Backend Engineering & System Design
# Open to collaborating on backend projects
```

## `~/connect`

<div align="center">

<a href="https://github.com/sanishil"><img src="https://img.shields.io/badge/GitHub-sanishil-0d1117?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://linkedin.com/in/sanishil"><img src="https://img.shields.io/badge/LinkedIn-sanishil-0d1117?style=for-the-badge&logo=linkedin&logoColor=0A66C2"/></a>
<a href="https://sanishil.site.je"><img src="https://img.shields.io/badge/Portfolio-sanishil.site.je-0d1117?style=for-the-badge&logo=google-chrome&logoColor=00F5A0"/></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00F5A0,50:0b3d2e,100:0d1117&height=140&section=footer" width="100%"/>

</div>
