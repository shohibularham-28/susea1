<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Ulangan Susulan — Narrative Text: Legend</title>
<style>
  :root{
    --bg1:#0f172a;
    --bg2:#1e293b;
    --card:#ffffff;
    --accent:#7c3aed;
    --accent2:#4f46e5;
    --correct:#16a34a;
    --wrong:#dc2626;
    --text:#1e293b;
    --muted:#64748b;
    --radius:16px;
  }
  *{box-sizing:border-box;}
  html,body{
    margin:0;padding:0;
    -webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;
    -webkit-touch-callout:none;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    background:linear-gradient(160deg,var(--bg1),var(--bg2) 60%,#312e81);
    color:var(--text);
    min-height:100vh;
  }
  img{-webkit-user-drag:none;}
  ::selection{background:transparent;}

  header.top{
    position:sticky;top:0;z-index:50;
    background:rgba(15,23,42,0.92);
    backdrop-filter:blur(6px);
    padding:14px 16px 10px;
    color:#fff;
    box-shadow:0 4px 18px rgba(0,0,0,0.25);
  }
  header.top h1{
    font-size:16px;margin:0 0 2px;font-weight:700;letter-spacing:.2px;
  }
  header.top p{margin:0;font-size:12px;color:#cbd5e1;}
  .progress-wrap{
    margin-top:10px;height:8px;border-radius:99px;background:#334155;overflow:hidden;
  }
  .progress-bar{
    height:100%;width:0%;background:linear-gradient(90deg,#a78bfa,#818cf8);
    transition:width .35s ease;
  }
  .progress-label{
    display:flex;justify-content:space-between;font-size:11px;color:#94a3b8;margin-top:6px;
  }

  main{
    max-width:640px;margin:0 auto;padding:16px 14px 120px;
  }

  .name-card{
    background:var(--card);border-radius:var(--radius);
    padding:18px;margin-bottom:16px;
    box-shadow:0 10px 30px rgba(0,0,0,0.25);
  }
  .name-card label{
    display:block;font-size:12px;color:var(--muted);margin-bottom:4px;font-weight:600;
  }
  .name-card input{
    -webkit-user-select:text;-moz-user-select:text;user-select:text;
    width:100%;padding:10px 12px;border-radius:10px;border:1.5px solid #e2e8f0;
    font-size:15px;margin-bottom:12px;background:#f8fafc;
  }
  .name-card input:focus{outline:none;border-color:var(--accent);background:#fff;}

  .part-title{
    color:#fff;font-size:13px;font-weight:800;letter-spacing:.5px;
    text-transform:uppercase;margin:18px 0 3px;padding-left:4px;
    display:flex;align-items:center;gap:8px;
  }
  .part-title .dot{
    width:8px;height:8px;border-radius:50%;background:#a78bfa;flex:none;
  }
  .part-desc{
    color:#cbd5e1;font-size:12px;margin:0 0 8px;padding-left:20px;
  }

  .qcard{
    background:var(--card);border-radius:var(--radius);padding:12px 16px 10px;
    margin-bottom:8px;box-shadow:0 8px 22px rgba(0,0,0,0.18);
    border:1.5px solid transparent;
    transition:border-color .2s;
  }
  .qcard.answered{border-color:#ede9fe;}
  .qtext{
    font-size:14.5px;line-height:1.35;margin:0 0 1px;font-weight:600;color:#0f172a;
  }
  .reading{
    font-size:13.5px;line-height:1.4;color:#334155;background:#f8fafc;
    border-left:4px solid #c4b5fd;padding:8px 10px;border-radius:8px;
    margin-bottom:6px;
  }
  .reading b{color:#4f46e5;}
  .qnum-badge{
    display:inline-block;background:var(--accent2);color:#fff;font-size:11px;
    font-weight:800;padding:2px 8px;border-radius:99px;margin-bottom:4px;
  }

  .opt{
    display:flex;align-items:flex-start;gap:10px;
    padding:8px 12px;border-radius:12px;border:1.5px solid #e2e8f0;
    margin-top:5px;cursor:pointer;transition:.15s;background:#fff;
  }
  .opt:active{transform:scale(0.985);}
  .opt input{margin-top:2px;pointer-events:none;flex:none;}
  .opt span.txt{font-size:13.8px;line-height:1.3;color:#1e293b;}
  .opt.selected{
    border-color:var(--accent);background:#f5f3ff;
  }
  .opt.correct{
    border-color:var(--correct)!important;background:#f0fdf4!important;
  }
  .opt.wrong{
    border-color:var(--wrong)!important;background:#fef2f2!important;
  }
  .opt .letter{
    flex:none;width:22px;height:22px;border-radius:7px;background:#eef2ff;color:#4f46e5;
    font-size:11.5px;font-weight:800;display:flex;align-items:center;justify-content:center;
    margin-top:0px;
  }
  .opt.correct .letter{background:var(--correct);color:#fff;}
  .opt.wrong .letter{background:var(--wrong);color:#fff;}

  .tf-row{display:flex;gap:10px;margin-top:6px;}
  .tf-btn{
    flex:1;text-align:center;padding:11px 0;border-radius:12px;border:1.5px solid #e2e8f0;
    font-weight:800;font-size:13px;letter-spacing:.5px;color:#475569;background:#fff;cursor:pointer;
  }
  .tf-btn.selected{border-color:var(--accent);background:#f5f3ff;color:var(--accent2);}
  .tf-btn.correct{border-color:var(--correct)!important;background:#f0fdf4!important;color:var(--correct)!important;}
  .tf-btn.wrong{border-color:var(--wrong)!important;background:#fef2f2!important;color:var(--wrong)!important;}

  .feedback{
    margin-top:8px;font-size:12.5px;padding:9px 11px;border-radius:9px;
    display:none;
  }
  .feedback.show{display:block;}
  .feedback.ok{background:#f0fdf4;color:#166534;}
  .feedback.no{background:#fef2f2;color:#991b1b;}

  .hint-multi{font-size:11px;color:var(--muted);margin:0 0 2px;font-style:italic;}

  footer.bar{
    position:fixed;bottom:0;left:0;right:0;
    background:rgba(15,23,42,0.95);backdrop-filter:blur(8px);
    padding:12px 16px calc(12px + env(safe-area-inset-bottom));
    display:flex;gap:10px;box-shadow:0 -6px 20px rgba(0,0,0,0.3);
    z-index:60;
  }
  .btn{
    flex:1;padding:13px 0;border-radius:12px;border:none;font-size:14.5px;font-weight:800;
    cursor:pointer;letter-spacing:.2px;
  }
  .btn-primary{background:linear-gradient(90deg,var(--accent2),var(--accent));color:#fff;}
  .btn-primary:disabled{opacity:.4;}
  .btn-ghost{background:#334155;color:#e2e8f0;flex:0 0 auto;padding:13px 18px;}

  .result-card{
    background:var(--card);border-radius:var(--radius);padding:26px 20px;text-align:center;
    box-shadow:0 10px 30px rgba(0,0,0,0.25);margin-top:10px;
  }
  .result-score{
    font-size:44px;font-weight:900;background:linear-gradient(90deg,var(--accent2),var(--accent));
    -webkit-background-clip:text;background-clip:text;color:transparent;margin:6px 0;
  }
  .result-sub{color:var(--muted);font-size:13.5px;margin-bottom:14px;}
  .breakdown{
    text-align:left;background:#f8fafc;border-radius:12px;padding:12px 14px;margin-top:14px;font-size:13px;
  }
  .breakdown div{display:flex;justify-content:space-between;padding:5px 0;border-bottom:1px dashed #e2e8f0;}
  .breakdown div:last-child{border-bottom:none;}

  .hidden{display:none!important;}

  @media print{
    html,body{display:none!important;}
  }

  .blur-protect{
    filter:blur(0px);
    transition:filter .15s;
  }
  body.blurred .blur-protect{
    filter:blur(18px) brightness(0.6);
  }

  #screenshotOverlay{
    position:fixed;inset:0;z-index:9999;
    background:rgba(15,23,42,0.97);
    display:none;
    align-items:center;justify-content:center;
    text-align:center;color:#fff;
    padding:30px;
  }
  #screenshotOverlay.show{display:flex;}
  #screenshotOverlay .box{
    max-width:320px;
  }
  #screenshotOverlay .icon{font-size:44px;margin-bottom:14px;}
  #screenshotOverlay h2{font-size:18px;margin:0 0 8px;}
  #screenshotOverlay p{font-size:13px;color:#cbd5e1;line-height:1.5;margin:0;}
</style>
</head>
<body oncontextmenu="return false;" oncopy="return false;" oncut="return false;" onpaste="return false;">

<div id="screenshotOverlay">
  <div class="box">
    <div class="icon">🚫</div>
    <h2>Screenshot Tidak Diizinkan</h2>
    <p>Halaman ujian ini dilindungi. Mohon jangan mengambil screenshot atau merekam layar selama mengerjakan soal.</p>
  </div>
</div>

<div class="blur-protect" id="protectedContent">

<header class="top">
  <h1>📖 Ulangan Susulan — Narrative Text: Legend</h1>
  <p id="progressText">0 / 30 dijawab</p>
  <div class="progress-wrap"><div class="progress-bar" id="progressBar"></div></div>
</header>

<main id="mainArea">
  <div class="name-card">
    <label>Nama</label>
    <input type="text" id="studentName" placeholder="Tulis nama kamu di sini">
    <label>Kelas</label>
    <input type="text" id="studentClass" placeholder="Tulis kelas kamu di sini">
  </div>
  <div id="quizContainer"></div>

  <div class="qcard" style="text-align:center;">
    <button class="btn btn-primary" id="submitBtn" style="width:100%;">✅ Submit</button>
  </div>

  <div id="resultArea" class="hidden"></div>
</main>

<footer class="bar">
  <button class="btn btn-ghost" id="resetBtn">↺ Ulangi</button>
  <button class="btn btn-primary" id="scrollTopBtn">⬆ Ke Atas</button>
</footer>

</div>

<script>
// ---------- Data Soal ----------
const DATA = [
  // PART 1
  {part:1, type:'single', num:1, text:'Choose the sentence that best expresses the main idea of the paragraph.',
   opts:{A:'The villagers placed flowers beside the old well every morning.',B:'The old well stood near a group of houses.',C:'The villagers became anxious when the old well suddenly stopped giving water.',D:'A mysterious event at the old well caused the village to change its attitude toward water.'},
   answer:'D'},
  {part:1, type:'single', num:2, text:'Choose the sentence that best expresses the main idea of the paragraph.',
   opts:{A:'A young trader crossed the eastern hills before sunset.',B:'The trader found a strange compass inside an abandoned hut.',C:'He usually traveled alone because he disliked crowded roads.',D:"The trader's decision to trust a mysterious compass helped him survive a difficult journey."},
   answer:'D'},
  {part:1, type:'single', num:3, text:'Choose the sentence that best expresses the main idea of the paragraph.',
   opts:{A:'Several birds gathered around the ancient tree.',B:'The tree had very wide branches.',C:'A girl visited the tree after hearing a strange sound.',D:'A mysterious tree taught the villagers an important lesson about protecting their forest.'},
   answer:'D'},
  {part:1, type:'single', num:4, text:'Choose the sentence that best expresses the main idea of the paragraph.',
   opts:{A:'The prince often visited the northern fields.',B:'Farmers planted corn near the palace.',C:'The prince owned a collection of silver cups.',D:"The prince's selfish choice caused the kingdom to lose a valuable natural blessing."},
   answer:'D'},
  {part:1, type:'single', num:5, text:'Choose the sentence that best expresses the main idea of the paragraph.',
   opts:{A:'The traveler walked beside a narrow river.',B:'He carried a small wooden box in his bag.',C:'An old woman lived near the river.',D:'The traveler learned that helping a stranger could lead to an unexpected reward.'},
   answer:'D'},

  // PART 2
  {part:2, type:'single', num:6,
   reading:'<b>Text 1 — The Legend of the Amber Bell</b><br>Long ago, a village stood between two wooded hills. At the center of the village hung an amber bell that was said to ring whenever the community faced an unseen danger. For many years, the villagers ignored the old story. One evening, a young baker named Sena heard the bell ring although nobody had touched it. She warned the villagers and asked them to move their animals to higher ground. Before midnight, heavy rain caused a nearby stream to overflow. Because the animals had already been moved, the villagers suffered little loss.',
   text:'What is the main idea of the text?',
   opts:{A:'A baker discovered a valuable bell in the hills.',B:'A mysterious bell warned a village about danger, and a young baker acted on the warning.',C:'The villagers built a new stream after a heavy rain.',D:'The amber bell was stolen by a group of travelers.',E:'The villagers ignored Sena because she wanted to become famous.'},
   answer:'B'},
  {part:2, type:'single', num:7,
   reading:'<b>Text 2 — The Legend of the Moon Orchard</b><br>According to an old valley legend, fruit trees in a hidden orchard produced fruit only for people who shared what they had. A poor gardener named Orin once found the orchard after helping an exhausted traveler. He picked only a few fruits and brought them home to his neighbors. The next morning, more fruit had appeared on the trees. Orin continued sharing the harvest, and the orchard remained abundant. When another gardener tried to take all the fruit for himself, the trees produced nothing.',
   text:'What is the main idea of the text?',
   opts:{A:"A gardener discovered that sharing was connected to the orchard's abundance.",B:'A traveler planted fruit trees in a poor valley.',C:'The orchard disappeared because Orin stopped gardening.',D:'The villagers refused to share fruit with strangers.',E:"A gardener became wealthy by selling all the orchard's fruit."},
   answer:'A'},
  {part:2, type:'single', num:8,
   reading:'<b>Text 3 — The Legend of the Reed Boat</b><br>In a remote marshland, people told a story about a reed boat that appeared whenever someone was willing to help a stranger. One afternoon, a young fisherman named Vale found an old traveler stranded on a muddy bank. Vale carried the traveler to a dry place and shared his food. As darkness fell, a small boat made of reeds floated toward them. Vale and the traveler used it to cross the marsh safely. The villagers later said the boat was a reward for compassion.',
   text:'What is the main idea of the text?',
   opts:{A:'A fisherman learned how to build boats from reeds.',B:'A traveler taught villagers how to cross a marsh.',C:'A mysterious reed boat appeared after a fisherman showed compassion.',D:'The villagers stopped fishing because the marsh became dangerous.',E:'A reed boat carried valuable goods across the marsh.'},
   answer:'C'},
  {part:2, type:'single', num:9,
   reading:'<b>Text 4 — The Legend of the Copper Hill</b><br>Many generations ago, a hill near a farming settlement was covered with small copper-colored stones. The villagers believed the stones protected the soil from becoming dry. During a long drought, a wealthy merchant ordered workers to collect the stones because he thought they were valuable. Soon, the fields around the hill became dusty and difficult to farm. Realizing their mistake, the villagers returned the stones to the hill. After the next rain, the soil slowly became fertile again.',
   text:'What is the main idea of the text?',
   opts:{A:'A merchant discovered a copper mine beneath a village.',B:'The villagers became wealthy by selling stones.',C:'The hill was dangerous because it contained metal.',D:"The legend explains how removing the hill's stones harmed the land and why they were restored.",E:'Farmers abandoned their fields during a long drought.'},
   answer:'D'},
  {part:2, type:'single', num:10,
   reading:'<b>Text 5 — The Legend of the Star Weaver</b><br>An old coastal legend tells of a woman named Ilya who wove fishing nets for poor families. One winter, the sea became unusually dark, and fishermen could not see the shoreline at night. Ilya placed tiny shells that reflected moonlight along the beach. The fishermen could then find their way home. The villagers later said that, on clear nights, the shells appeared like small stars. The tradition of placing shells along the shore continued for generations.',
   text:'What is the main idea of the text?',
   opts:{A:'A woman created a tradition that helped fishermen find their way home at night.',B:'Fishermen discovered a new source of valuable shells.',C:'The sea became bright because of a magical storm.',D:'The villagers stopped fishing during winter.',E:'Ilya became a famous trader because she sold shells.'},
   answer:'A'},

  // PART 3
  {part:3, type:'single', num:11,
   reading:'<b>Text A — The Legend of the Echoing Fig Tree</b><br>In a hillside settlement, an enormous fig tree stood beside an old footpath. People said that the tree repeated the last kind words spoken beneath its branches. Most villagers considered the story a children\'s tale. One afternoon, a boy named Raka found an elderly traveler struggling with a heavy basket. Raka helped carry the basket to the village and thanked the traveler for trusting him. As they passed the fig tree on the way home, the tree seemed to repeat Raka\'s words. The villagers were surprised. From then on, they began to speak more kindly to one another beneath the tree, hoping its echo would remind them of the value of kindness.',
   text:'Why did Raka help the elderly traveler?',
   opts:{A:'He wanted to receive a valuable gift.',B:'He was asked by the village chief to help the traveler.',C:'He noticed that the traveler was struggling with a heavy basket.',D:'He wanted to test whether the fig tree could speak.',E:'He needed the traveler to show him a hidden path.'},
   answer:'C'},
  {part:3, type:'single', num:12,
   text:"What did the villagers do after the fig tree seemed to repeat Raka's words?",
   opts:{A:'They cut down the fig tree.',B:'They began speaking more kindly to one another.',C:'They stopped using the old footpath.',D:'They asked Raka to leave the village.',E:'They planted a new fig tree beside the river.'},
   answer:'B'},
  {part:3, type:'single', num:13,
   reading:'<b>Text B — The Legend of the Misty Path</b><br>A merchant named Elian once traveled through a mountain valley where thick mist often covered the roads. Local people believed that a pale bird appeared to travelers who were about to choose an unsafe path. One evening, Elian saw the bird flying toward a narrow road. He followed it in the opposite direction and reached a small settlement before dark. The next morning, he learned that a rockslide had blocked the narrow road during the night. Elian believed the bird had guided him away from danger.',
   text:'What can be inferred about the pale bird?',
   opts:{A:'It probably appeared as a warning to travelers.',B:'It belonged to Elian.',C:'It always flew over the safest road in the valley.',D:'It wanted to lead travelers toward rockslides.',E:'It appeared only during the rainy season.'},
   answer:'A'},
  {part:3, type:'single', num:14,
   text:'Why did Elian believe the bird had helped him?',
   opts:{A:'The bird carried him to the settlement.',B:'The bird told him about the rockslide.',C:'He later learned that the road he avoided had been blocked.',D:'The villagers said that Elian owned the bird.',E:"He found food near the bird's nest."},
   answer:'C'},
  {part:3, type:'single', num:15,
   text:"Which statement best describes Elian's decision?",
   opts:{A:'He ignored the unusual sign and continued on the narrow road.',B:'He followed the bird directly into the mist.',C:"He changed his route after noticing the bird's behavior.",D:'He returned to the market to buy another map.',E:'He asked the villagers to remove the mountain road.'},
   answer:'C'},

  // PART 4 (multi)
  {part:4, type:'multi', num:16,
   reading:'<b>Text A — The Legend of the Silver Seed</b><br>In a dry farming village, a girl named Nemi received one silver seed from a quiet stranger. The stranger told her that the seed would grow only if its harvest was shared. Nemi planted it near the village well. A month later, a tall plant grew and produced enough grain for many families. Nemi kept a small portion for her own family and distributed the rest. The following season, the plant disappeared, but the villagers began sharing their harvests more willingly because they remembered Nemi\'s example.',
   text:'Which statements are supported by the text?',
   opts:{A:'Nemi received one silver seed.',B:'The stranger told Nemi to keep the harvest for herself.',C:'The plant produced enough grain for many families.',D:'Nemi distributed part of the harvest.'},
   answer:['A','C','D']},
  {part:4, type:'multi', num:17,
   text:'Which lessons can be learned from the legend?',
   opts:{A:'Sharing can strengthen a community.',B:'A person should always keep unexpected gifts.',C:"One person's example can influence others.",D:'Helping others is useful only when a reward is guaranteed.'},
   answer:['A','C']},
  {part:4, type:'multi', num:18,
   text:'Which events happened in the story?',
   opts:{A:'Nemi planted the silver seed.',B:'The plant produced grain.',C:'The villagers sold the entire harvest to a merchant.',D:'The plant disappeared after the following season.'},
   answer:['A','B','D']},
  {part:4, type:'multi', num:19,
   reading:'<b>Text B — The Legend of the Listening Cave</b><br>A cave beside a mountain was believed to repeat only truthful words. A young hunter named Sava entered the cave while searching for a lost goat. Inside, he found an old traveler who asked whether Sava had seen a hidden path. Sava honestly said that he had not. The cave repeated his answer clearly. Later, Sava discovered the traveler was looking for a safe route to the village. Sava then returned and guided him there. The villagers remembered the story as a lesson that honesty could build trust.',
   text:'Which statements are true according to the text?',
   opts:{A:'Sava entered the cave while searching for a goat.',B:'Sava lied about seeing a hidden path.',C:"The cave repeated Sava's truthful answer.",D:'Sava later helped the traveler find a safe route.'},
   answer:['A','C','D']},
  {part:4, type:'multi', num:20,
   text:'Which ideas are implied by the legend?',
   opts:{A:'Honesty can help people trust one another.',B:'Truthful answers may be valuable even when they seem simple.',C:'Sava helped the traveler only because he wanted money.',D:'The villagers considered honesty an important quality.'},
   answer:['A','B','D']},

  // PART 5 (true/false)
  {part:5, type:'tf', num:21,
   reading:'<b>Text 1 — The Legend of the Glass Kite</b><br>A village near the sea once suffered because fishermen could not tell when strong winds were approaching. A girl named Mara made a kite from thin cloth and pieces of clear glass. Whenever the wind became dangerous, the kite produced a sharp sound. The villagers used the sound as a warning and brought their boats closer to shore. After Mara grew older, the villagers taught younger children how to make similar warning kites.',
   text:'Mara made the first warning kite from cloth and pieces of glass.', answer:'TRUE'},
  {part:5, type:'tf', num:22,
   text:'The kite was used mainly to entertain children during calm weather.', answer:'FALSE'},
  {part:5, type:'tf', num:23,
   reading:'<b>Text 2 — The Legend of the Sleeping Lake</b><br>An old legend says that a lake became completely still whenever people forgot to care for the land around it. One summer, villagers cut many trees near the lake and left rubbish along its shore. The water soon became unusually quiet. A farmer named Tera organized a clean-up and encouraged the villagers to plant new trees. Over time, the lake became lively again, and the villagers believed it had awakened.',
   text:'The villagers improved the area around the lake by cleaning it and planting trees.', answer:'TRUE'},
  {part:5, type:'tf', num:24,
   text:'The lake became still because the villagers planted too many trees.', answer:'FALSE'},
  {part:5, type:'tf', num:25,
   reading:'<b>Text 3 — The Legend of the Bronze Sparrow</b><br>A bronze statue of a sparrow stood above the gate of an ancient town. According to local legend, the statue turned toward the direction from which danger would come. One morning, it faced west even though danger had never come from that direction before. The town leader sent scouts west and discovered that a bridge had collapsed on the main road. Travelers were redirected to a safer route.',
   text:"The statue's unusual movement led the town leader to investigate the western road.", answer:'TRUE'},
  {part:5, type:'tf', num:26,
   text:'The collapsed bridge was discovered on the eastern road.', answer:'FALSE'},
  {part:5, type:'tf', num:27,
   reading:'<b>Text 4 — The Legend of the Rain Drum</b><br>In a mountain village, a large drum was kept in a small wooden shelter. People believed that the drum would sound when the first rain of the season was near. One year, the villagers heard the drum at dawn. Instead of waiting, they repaired the channels that carried water to their fields. Heavy rain arrived two days later, and the repaired channels helped prevent the fields from flooding.',
   text:'The villagers repaired the water channels after hearing the drum.', answer:'TRUE'},
  {part:5, type:'tf', num:28,
   text:'The heavy rain arrived on the same day that the drum sounded.', answer:'FALSE'},
  {part:5, type:'tf', num:29,
   reading:'<b>Text 5 — The Legend of the Willow Lantern</b><br>A river village once used lanterns to guide boats through a bend that was difficult to navigate at night. A young carpenter named Lio noticed that the old lantern posts were too weak. He built new wooden frames and placed them higher above the riverbank. During the next storm, the new frames remained standing and continued to guide the boats. The villagers later said that Lio\'s careful work had protected the community.',
   text:'Lio strengthened the lantern posts before the next storm.', answer:'TRUE'},
  {part:5, type:'tf', num:30,
   text:'The new lantern frames fell into the river during the storm.', answer:'FALSE'},
];

const PART_INFO = {
  1:{title:'Part 1 — Identifying the Main Sentence', desc:'Pilih SATU jawaban yang benar (A–D).'},
  2:{title:'Part 2 — Identifying the Main Idea', desc:'Pilih SATU jawaban yang benar (A–E).'},
  3:{title:'Part 3 — Textual & Inferential Information', desc:'Pilih SATU jawaban yang benar (A–E).'},
  4:{title:'Part 4 — Multiple Choice, Multiple Answers', desc:'Pilih SEMUA jawaban yang benar.'},
  5:{title:'Part 5 — True or False', desc:'Tentukan TRUE atau FALSE untuk setiap pernyataan.'}
};

const userAnswers = {}; // num -> string or array
let submitted = false;

const container = document.getElementById('quizContainer');
let lastPart = 0;

DATA.forEach(q=>{
  if(q.part !== lastPart){
    lastPart = q.part;
    const pt = document.createElement('div');
    pt.className='part-title';
    pt.innerHTML = `<span class="dot"></span>${PART_INFO[q.part].title}`;
    container.appendChild(pt);
    const pd = document.createElement('p');
    pd.className='part-desc';
    pd.textContent = PART_INFO[q.part].desc;
    container.appendChild(pd);
  }

  const card = document.createElement('div');
  card.className='qcard';
  card.id = 'card-'+q.num;

  let html = '';
  html += `<div class="qnum-badge">Soal ${q.num}</div>`;
  if(q.reading){ html += `<div class="reading">${q.reading}</div>`; }
  html += `<p class="qtext">${q.text}</p>`;

  if(q.type==='single'){
    Object.keys(q.opts).forEach(letter=>{
      html += `<div class="opt" data-letter="${letter}" onclick="selectSingle(${q.num},'${letter}')">
        <div class="letter">${letter}</div><span class="txt">${q.opts[letter]}</span></div>`;
    });
  } else if(q.type==='multi'){
    html += `<p class="hint-multi">* Bisa pilih lebih dari satu jawaban</p>`;
    Object.keys(q.opts).forEach(letter=>{
      html += `<div class="opt" data-letter="${letter}" onclick="toggleMulti(${q.num},'${letter}')">
        <div class="letter">${letter}</div><span class="txt">${q.opts[letter]}</span></div>`;
    });
  } else if(q.type==='tf'){
    html += `<div class="tf-row">
      <div class="tf-btn" data-val="TRUE" onclick="selectTF(${q.num},'TRUE')">TRUE</div>
      <div class="tf-btn" data-val="FALSE" onclick="selectTF(${q.num},'FALSE')">FALSE</div>
    </div>`;
  }
  html += `<div class="feedback" id="fb-${q.num}"></div>`;

  card.innerHTML = html;
  container.appendChild(card);
});

function updateProgress(){
  const answered = Object.keys(userAnswers).filter(k=>{
    const v = userAnswers[k];
    return Array.isArray(v) ? v.length>0 : !!v;
  }).length;
  document.getElementById('progressText').textContent = answered + ' / 30 dijawab';
  document.getElementById('progressBar').style.width = (answered/30*100)+'%';
}

function selectSingle(num, letter){
  if(submitted) return;
  userAnswers[num] = letter;
  const card = document.getElementById('card-'+num);
  card.classList.add('answered');
  card.querySelectorAll('.opt').forEach(o=>{
    o.classList.toggle('selected', o.dataset.letter===letter);
  });
  updateProgress();
}

function toggleMulti(num, letter){
  if(submitted) return;
  if(!userAnswers[num]) userAnswers[num] = [];
  const arr = userAnswers[num];
  const idx = arr.indexOf(letter);
  if(idx>-1){ arr.splice(idx,1); } else { arr.push(letter); }
  const card = document.getElementById('card-'+num);
  card.classList.toggle('answered', arr.length>0);
  card.querySelectorAll('.opt').forEach(o=>{
    o.classList.toggle('selected', arr.includes(o.dataset.letter));
  });
  updateProgress();
}

function selectTF(num, val){
  if(submitted) return;
  userAnswers[num] = val;
  const card = document.getElementById('card-'+num);
  card.classList.add('answered');
  card.querySelectorAll('.tf-btn').forEach(b=>{
    b.classList.toggle('selected', b.dataset.val===val);
  });
  updateProgress();
}

function arraysEqual(a,b){
  if(a.length!==b.length) return false;
  const sa=[...a].sort(), sb=[...b].sort();
  return sa.every((v,i)=>v===sb[i]);
}

document.getElementById('submitBtn').addEventListener('click', ()=>{
  submitted = true;
  let correctCount = 0;
  const byPart = {1:{c:0,t:0},2:{c:0,t:0},3:{c:0,t:0},4:{c:0,t:0},5:{c:0,t:0}};

  DATA.forEach(q=>{
    byPart[q.part].t++;
    const card = document.getElementById('card-'+q.num);
    const ua = userAnswers[q.num];
    let isCorrect = false;

    if(q.type==='single'){
      isCorrect = ua === q.answer;
      card.querySelectorAll('.opt').forEach(o=>{ o.onclick = null; });
    } else if(q.type==='multi'){
      const arr = ua || [];
      isCorrect = arraysEqual(arr, q.answer);
      card.querySelectorAll('.opt').forEach(o=>{ o.onclick = null; });
    } else if(q.type==='tf'){
      isCorrect = ua === q.answer;
      card.querySelectorAll('.tf-btn').forEach(b=>{ b.onclick = null; });
    }

    if(isCorrect){ correctCount++; byPart[q.part].c++; }
  });

  document.getElementById('submitBtn').disabled = true;
  document.getElementById('submitBtn').textContent = '✅ Sudah Disubmit';

  const name = document.getElementById('studentName').value.trim() || '(tanpa nama)';
  const cls = document.getElementById('studentClass').value.trim() || '(tanpa kelas)';
  const score = Math.round((correctCount/30)*100);

  const resultArea = document.getElementById('resultArea');
  resultArea.classList.remove('hidden');
  resultArea.innerHTML = `
    <div class="result-card">
      <div style="font-size:15px;font-weight:700;color:#0f172a;">${name} — ${cls}</div>
      <div style="font-size:44px;margin:14px 0;">✅</div>
      <div class="result-sub" style="font-size:14px;">Jawaban kamu telah berhasil disubmit.</div>
      <div id="sendStatus" style="margin-top:12px;font-size:12.5px;color:#64748b;">⏳ Mengirim hasil ke guru...</div>
    </div>`;
  resultArea.scrollIntoView({behavior:'smooth', block:'start'});

  // ---------- Susun ringkasan lengkap semua jawaban + skor ----------
  let summaryLines = [];
  summaryLines.push(`Nama: ${name} | Kelas: ${cls} | Skor: ${score} (${correctCount}/30)`);
  DATA.forEach(q=>{
    const ua = userAnswers[q.num];
    let uaText;
    if(q.type==='multi'){
      uaText = (ua && ua.length) ? ua.sort().join(',') : '-';
    } else {
      uaText = ua || '-';
    }
    const correctText = q.type==='multi' ? q.answer.join(',') : q.answer;
    const mark = (q.type==='multi') ? (arraysEqual(ua||[], q.answer) ? 'Benar' : 'Salah')
               : (ua===q.answer ? 'Benar' : 'Salah');
    summaryLines.push(`No.${q.num}: ${uaText} (Kunci: ${correctText}) - ${mark}`);
  });
  const fullSummary = summaryLines.join(' || ');

  sendToGoogleForm(fullSummary);
});

function sendToGoogleForm(summaryText){
  const FORM_ACTION = 'https://docs.google.com/forms/d/e/1FAIpQLSfkMKtrHuM_qcc_mhOfWYsyp5PXr21V0kOZqWwVJF8bMuO5eg/formResponse';
  const ENTRY_ID = 'entry.553083686';

  const iframe = document.createElement('iframe');
  iframe.name = 'hidden_submit_frame';
  iframe.style.display = 'none';
  document.body.appendChild(iframe);

  const form = document.createElement('form');
  form.action = FORM_ACTION;
  form.method = 'POST';
  form.target = 'hidden_submit_frame';

  const input = document.createElement('input');
  input.type = 'hidden';
  input.name = ENTRY_ID;
  input.value = summaryText;
  form.appendChild(input);

  document.body.appendChild(form);
  form.submit();

  setTimeout(()=>{
    const st = document.getElementById('sendStatus');
    if(st){ st.textContent = '✅ Hasil berhasil dikirim ke guru.'; }
    document.body.removeChild(form);
    document.body.removeChild(iframe);
  }, 1200);
}

document.getElementById('resetBtn').addEventListener('click', ()=>{
  location.reload();
});
document.getElementById('scrollTopBtn').addEventListener('click', ()=>{
  window.scrollTo({top:0, behavior:'smooth'});
});

// ---------- Proteksi anti select / copy / print ----------
document.addEventListener('contextmenu', e=>e.preventDefault());
document.addEventListener('selectstart', e=>e.preventDefault());
document.addEventListener('copy', e=>e.preventDefault());
document.addEventListener('cut', e=>e.preventDefault());
document.addEventListener('dragstart', e=>e.preventDefault());
document.addEventListener('keydown', e=>{
  const k = e.key.toLowerCase();
  if((e.ctrlKey||e.metaKey) && ['c','x','p','s','u'].includes(k)){
    e.preventDefault();
  }
  if(e.key === 'F12' || (e.ctrlKey && e.shiftKey && ['i','j','c'].includes(k))){
    e.preventDefault();
  }
});
window.addEventListener('beforeprint', e=>{
  document.body.innerHTML = '<div style="padding:40px;text-align:center;font-family:sans-serif;">Mencetak halaman ini tidak diizinkan.</div>';
});

// ---------- Upaya pencegahan screenshot (tidak 100% efektif) ----------
// Catatan: browser/OS tidak menyediakan API untuk benar-benar memblokir screenshot.
// Bagian ini hanya memberi hambatan tambahan (blur otomatis + peringatan).
const overlay = document.getElementById('screenshotOverlay');
let overlayTimer = null;

function showScreenshotWarning(duration){
  overlay.classList.add('show');
  document.body.classList.add('blurred');
  clearTimeout(overlayTimer);
  overlayTimer = setTimeout(()=>{
    overlay.classList.remove('show');
    document.body.classList.remove('blurred');
  }, duration || 2500);
}

// Deteksi tombol PrintScreen (desktop)
document.addEventListener('keyup', e=>{
  if(e.key === 'PrintScreen'){
    showScreenshotWarning(3000);
  }
});
document.addEventListener('keydown', e=>{
  // Windows Snipping Tool / Win+Shift+S tidak bisa dideteksi langsung,
  // tapi kombinasi umum lain kita tangkap sebagai sinyal
  if((e.metaKey && e.shiftKey && e.key.toLowerCase()==='s')){
    showScreenshotWarning(3000);
  }
});

// Blur otomatis saat tab/app kehilangan fokus (indikasi pindah ke app screenshot/recorder)
document.addEventListener('visibilitychange', ()=>{
  if(document.hidden){
    document.body.classList.add('blurred');
  } else {
    setTimeout(()=>document.body.classList.remove('blurred'), 400);
  }
});
window.addEventListener('blur', ()=>{
  document.body.classList.add('blurred');
});
window.addEventListener('focus', ()=>{
  setTimeout(()=>document.body.classList.remove('blurred'), 400);
});

</script>
</body>
</html>
