Leia isso em outros Idiomas: [русский](FAQru.md), [Français](FAQfr.md), [Nederlands](FAQnl.md), [Türkçe](FAQtr.md), [українська](FAQuk.md), [Polski](FAQpl.md)

# Perguntas frequentes

## Antes de fazer uma perguntar no GitHub ou Discord, por favor consulte isso.

<br>

### **1. De onde essa extensão recebe dados?**

Uma combinação das APIs do Google e dados extraídos.

Nós salvamos todos os dados disponiveis no nosso banco de dados pra isso ficar disponivel após a Google desligar o contador de dislikes na API deles.

<br>

### **2. Quantidade de dislikes do video não atualizando**

Por enquanto, os dislikes dos videos são mantidos em cache e não são atualizados tão frequentemente. Uma vez a cada 2-3 dias, no máximo.

Sim, não é o ideal, mas é o que tem que ser. Funcionando e melhorando conforme atualizamos.

<br>

### **3. Como que isso funciona?**

A extensão coleta o id do vídeo que você está assistindo, busca os dislikes (e outros campos como views, likes, etc) usando nossa API, se esse é a primeira vez que o vídeo foi retornando pela nossa API, ela vai usar a API do Youtube para buscar os dados, e então, armazenar os dados em um banco de dados para fins de cache (fica em cache por 2-3 dias) e arquivamento e retorna para você. A extensão então mostra os dislikes.

<br>

### **4. What will happen after the YouTube API stops returning the dislike count?**

The backend will switch to using a combination of archived dislike stats, estimates extrapolated from extension user data and estimates based on view/like ratios for videos whose dislikes weren't archived and for outdated dislike archives.

<br>

### **5. How is the dislike count calculated?**

RYD uses the votes from its users to extrapolate the dislike count.

- If the video was uploaded after the API was shut down:

  $$ \textup{RYD Dislike Count} = \left( \frac{\textup{RYD Users Dislike Count}}{\textup{RYD Users Like Count}} \right) \times \textup{Public Like Count} $$

- If the RYD database somehow had the actual like and dislike count (provided by the uploader or from the archive), the dislike count will be calculated based on both - the users' votes and the archived value. The archived value will have less influence on the final count as it ages.

<br>

---

Essa a This in video form

[![IReturn YouTube Dislike Explained](https://yt-embed.herokuapp.com/embed?v=GSmmtv-0yYQ)](https://www.youtube.com/watch?v=GSmmtv-0yYQ)

---

<br>

## I have security / privacy concerns

Leia [essa pagina](SECURITY-FAQpt_BR.md) para mais informações.
