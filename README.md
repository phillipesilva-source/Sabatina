<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dúvidas sobre a Sabatina Eleitoral 2026 — Salvador FM</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@600;700;800&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --navy-deep:#0a1638;
    --navy:#0f2358;
    --navy-card:#132a68;
    --blue:#2f5fe0;
    --cyan:#4fd8e8;
    --amber:#f2a93b;
    --ink:#0d1530;
    --paper:#f6f7fb;
    --slate:#8891ab;
    --line: rgba(255,255,255,0.10);
  }
  *{box-sizing:border-box;}
  body{margin:0;}
  html{scroll-behavior:smooth;}
  body{
    background:
      radial-gradient(1200px 600px at 50% -10%, #16306e 0%, var(--navy-deep) 55%),
      var(--navy-deep);
    color:#eef1fb;
    font-family:'Inter',system-ui,sans-serif;
    min-height:100vh;
    padding-bottom:80px;
  }
  .bg-rings{
    position:fixed; inset:0; z-index:0; pointer-events:none; overflow:hidden;
  }
  .bg-rings svg{position:absolute; top:-10%; left:50%; transform:translateX(-50%); opacity:0.35;}
  .ring{fill:none; stroke:var(--cyan); stroke-opacity:0.18;}
  .ring.b{stroke:var(--blue); stroke-opacity:0.14;}
  @keyframes pulse{
    0%,100%{ stroke-opacity:0.08; }
    50%{ stroke-opacity:0.22; }
  }
  .ring{ animation: pulse 6s ease-in-out infinite; }
  .ring:nth-child(2){ animation-delay:0.8s; }
  .ring:nth-child(3){ animation-delay:1.6s; }
  .ring:nth-child(4){ animation-delay:2.4s; }
  .ring:nth-child(5){ animation-delay:3.2s; }

  .wrap{position:relative; z-index:1; max-width:760px; margin:0 auto; padding:0 20px;}

  header{padding-top:56px; text-align:center;}
  .eyebrow{
    font-size:12px; letter-spacing:.18em; text-transform:uppercase;
    color:var(--cyan); font-weight:600; margin-bottom:10px;
  }
  .eyebrow::before{content:"● "; color:var(--amber);}
  h1{
    font-family:'Barlow Condensed',sans-serif;
    font-weight:800;
    text-transform:uppercase;
    letter-spacing:.01em;
    font-size:clamp(34px,7vw,58px);
    line-height:0.98;
    margin:0 0 6px;
  }
  h1 span{color:var(--amber);}
  .sub{color:var(--slate); font-size:15px; max-width:480px; margin:14px auto 0; line-height:1.5;}

  /* search */
  .search-shell{margin-top:38px; position:relative;}
  .search-box{
    display:flex; align-items:center; gap:12px;
    background:#ffffff; border-radius:999px;
    padding:8px 8px 8px 22px;
    box-shadow: 0 20px 50px -20px rgba(0,0,0,0.6), 0 0 0 1px rgba(255,255,255,0.06);
  }
  .search-box:focus-within{ box-shadow: 0 20px 50px -20px rgba(0,0,0,0.6), 0 0 0 2px var(--cyan); }
  .timer-icon{ position:relative; width:22px; height:22px; flex:0 0 auto; }
  .timer-icon svg{ width:100%; height:100%; }
  .ring-progress{
    stroke-dasharray: 56; stroke-dashoffset: 56;
    transform-origin:50% 50%; transform:rotate(-90deg);
    animation: tick 3s linear infinite;
  }
  @keyframes tick{ to{ stroke-dashoffset:0; } }
  #q{
    flex:1; border:none; outline:none; font-size:17px; font-family:'Inter',sans-serif;
    color:var(--ink); background:transparent; padding:12px 0;
  }
  #q::placeholder{ color:#a7adc2; }
  .go-btn{
    border:none; background:var(--navy); color:#fff; font-weight:600; font-size:14px;
    padding:12px 22px; border-radius:999px; cursor:pointer;
    transition: background .15s ease, transform .1s ease;
  }
  .go-btn:hover{ background:var(--blue); }
  .go-btn:active{ transform: scale(0.97); }

  .chips{display:flex; flex-wrap:wrap; gap:8px; justify-content:center; margin-top:20px;}
  .chip{
    font-size:13px; padding:7px 14px; border-radius:999px;
    border:1px solid var(--line); color:#cfd6ef; background:rgba(255,255,255,0.03);
    cursor:pointer; transition: all .15s ease; font-weight:500;
  }
  .chip:hover{ background:rgba(79,216,232,0.12); border-color:var(--cyan); color:#fff; }

  /* results */
  #results{ margin-top:36px; display:flex; flex-direction:column; gap:14px; }
  .hint{ text-align:center; color:var(--slate); font-size:13px; margin-top:28px; }

  .card{
    background:var(--navy-card);
    border:1px solid var(--line);
    border-radius:16px;
    padding:20px 22px;
    animation: rise .35s ease both;
  }
  @keyframes rise{ from{ opacity:0; transform:translateY(8px);} to{opacity:1; transform:translateY(0);} }
  .card-top{ display:flex; align-items:center; gap:10px; margin-bottom:10px; flex-wrap:wrap; }
  .badge{
    font-family:'Barlow Condensed',sans-serif;
    font-weight:700; font-size:13px; letter-spacing:.03em;
    background:var(--amber); color:#241505;
    padding:3px 10px; border-radius:7px;
  }
  .topic{ font-size:12px; color:var(--cyan); text-transform:uppercase; letter-spacing:.08em; font-weight:600; }
  .answer{ font-size:16px; line-height:1.55; color:#f1f3fc; }
  .no-result{
    text-align:center; padding:34px 20px; color:var(--slate);
    border:1px dashed var(--line); border-radius:16px; font-size:14px; line-height:1.6;
  }
  .no-result b{ color:#fff; }

  footer{
    max-width:760px; margin:64px auto 0; padding:22px 20px 0; text-align:center;
    border-top:1px solid var(--line); color:var(--slate); font-size:12.5px; line-height:1.7;
  }
  footer strong{ color:#c7cef0; }

  @media (prefers-reduced-motion: reduce){
    .ring, .ring-progress{ animation:none !important; }
  }
</style>
</head>
<body>

<div class="bg-rings" aria-hidden="true">
  <svg width="900" height="900" viewBox="0 0 900 900">
    <circle class="ring" cx="450" cy="450" r="120"/>
    <circle class="ring b" cx="450" cy="450" r="200"/>
    <circle class="ring" cx="450" cy="450" r="280"/>
    <circle class="ring b" cx="450" cy="450" r="360"/>
    <circle class="ring" cx="450" cy="450" r="440"/>
  </svg>
</div>

<div class="wrap">
  <header>
    <div class="eyebrow">Hora Eleitoral 2026 · Salvador FM 92.3</div>
    <h1>Dúvidas da<br><span>Sabatina</span></h1>
    <p class="sub">Digite sua pergunta sobre as regras da Sabatina Eleitoral e receba a resposta em linguagem simples, com o artigo do regulamento.</p>
  </header>

  <div class="search-shell">
    <div class="search-box">
      <span class="timer-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24">
          <circle cx="12" cy="12" r="9" fill="none" stroke="#dfe3f2" stroke-width="2"/>
          <circle class="ring-progress" cx="12" cy="12" r="9" fill="none" stroke="#2f5fe0" stroke-width="2"/>
          <line x1="12" y1="12" x2="12" y2="6.5" stroke="#0d1530" stroke-width="1.6" stroke-linecap="round"/>
        </svg>
      </span>
      <input id="q" type="text" placeholder="Ex: posso usar celular na sabatina?" autocomplete="off">
      <button class="go-btn" onclick="runSearch()">Buscar</button>
    </div>
    <div class="chips" id="chips"></div>
  </div>

  <div id="results"></div>
  <p class="hint" id="hint">Toque em um tema acima ou digite sua dúvida — a busca considera palavras parecidas mesmo sem acento.</p>
</div>

<footer>
  Respostas baseadas no <strong>Regulamento das Sabatinas Eleitorais 2026 — Salvador FM</strong> (118 artigos e 5 anexos).<br>
  Em caso de dúvida sobre um caso específico ou não coberto aqui, procure os canais oficiais da campanha/emissora previstos no Art. 114.
</footer>

<script>
// ---------- Base de conhecimento (regulamento resumido em linguagem simples) ----------
const KB = [
  { topic:"Objetivo", art:"Art. 1º a 3º", keywords:"objetivo finalidade proposito sabatina o que e eleicoes 2026 principios isonomia imparcialidade",
    answer:"A Sabatina é uma entrevista jornalística da Salvador FM com as candidaturas ao Governo da Bahia nas Eleições 2026, feita com isonomia entre os candidatos, independência editorial e respeito à legislação eleitoral." },
  { topic:"Transmissão ao vivo", art:"Art. 6º, 90 e 91", keywords:"transmissao ao vivo onde assistir dial fm youtube site aplicativo canal tempo real atraso",
    answer:"A Sabatina vai ao vivo pelo dial 92,3 FM, pelo site oficial, pelo aplicativo da Salvador FM e pelo canal oficial no YouTube, em tempo real, sem atraso intencional." },
  { topic:"Quem participa", art:"Art. 7º e 8º", keywords:"quem participa candidatos governador definicao candidaturas participantes criterios legais",
    answer:"Participam as candidaturas ao Governo do Estado da Bahia definidas pela Salvador FM, seguindo os critérios legais vigentes na data das Sabatinas." },
  { topic:"Sorteio da ordem", art:"Art. 9º", keywords:"sorteio ordem participacao reuniao data 10 de agosto quando decide quem entra primeiro gravacao do sorteio",
    answer:"A ordem de participação é definida por sorteio formal, feito na reunião oficial do dia 10/08/2026 às 15h na sede da Salvador FM, com todo o procedimento gravado. A gravação pode ser pedida pela campanha em até 2 dias úteis." },
  { topic:"Ausência na reunião do sorteio", art:"Art. 9º §6º e §7º", keywords:"ausencia reuniao sorteio nao foi nao compareceu representante invalida",
    answer:"Se a campanha não comparecer à reunião do sorteio, isso não invalida o resultado nem impede a candidatura de participar — desde que tenha sido convocada oficialmente." },
  { topic:"Confirmar participação", art:"Art. 10", keywords:"confirmar participacao prazo desistencia nao confirmou whatsapp email",
    answer:"A campanha precisa confirmar a participação até o prazo informado pela Salvador FM por e-mail, WhatsApp ou outro canal oficial. Quem não confirma no prazo é considerado desistente." },
  { topic:"Se o candidato faltar", art:"Art. 11", keywords:"faltou nao compareceu desistencia cadeira vazia mesa redonda ausencia do candidato",
    answer:"Se a candidatura desistir ou faltar, o programa acontece normalmente: a cadeira fica vazia, as perguntas previstas são lidas e o tempo restante vira uma mesa-redonda jornalística, sem favorecer nenhum lado." },
  { topic:"Troca pelo vice", art:"Art. 12", keywords:"vice governador substituicao trocar candidato substituir",
    answer:"O candidato a vice só pode substituir o titular com pedido formal da campanha e autorização prévia da Direção de Jornalismo. Quem entra segue as mesmas regras." },
  { topic:"Chegada ao estúdio", art:"Art. 13", keywords:"chegar horario antecedencia minutos estudio atraso chegou tarde",
    answer:"A candidatura deve chegar com pelo menos 45 minutos de antecedência do horário da transmissão. Chegar dentro do prazo é condição obrigatória para participar." },
  { topic:"Camarim e alinhamento", art:"Art. 14 e 15", keywords:"camarim alinhamento antes de entrar regras podem mudar negociar",
    answer:"Ao chegar, a candidatura é recebida pela produção e fica no camarim até ser levada ao estúdio. Pode haver um alinhamento operacional antes, mas nenhuma regra pode ser negociada ou alterada depois que a transmissão começa." },
  { topic:"Credenciamento", art:"Art. 16", keywords:"credenciamento acesso entrada quem controla",
    answer:"Não existe credenciamento formal; quem controla a entrada e a circulação de pessoas nas dependências é a equipe de produção da Salvador FM." },
  { topic:"Assessores e equipe de mídia", art:"Art. 17", keywords:"assessores acompanhantes quantos pode levar equipe fotografo imprensa propria",
    answer:"Cada candidatura pode levar até 3 assessores e 2 profissionais de mídia, mas dentro do estúdio só ficam 1 assessor e até 2 profissionais de mídia, só para fotos e redes sociais — sem interferir na condução do programa." },
  { topic:"Plateia", art:"Art. 18", keywords:"plateia publico presencial pode assistir ao vivo no estudio",
    answer:"Não é permitida plateia durante a Sabatina." },
  { topic:"Água/estrutura", art:"Art. 19", keywords:"agua estrutura disponibilizada",
    answer:"A Salvador FM disponibiliza água ao candidato durante sua permanência na emissora." },
  { topic:"Comunicação com a campanha", art:"Art. 20", keywords:"comunicacao equipe campanha durante sabatina falar com assessor celular escondido fone",
    answer:"Depois que a Sabatina começa, não é permitida nenhuma comunicação entre o candidato e sua equipe — nem verbal, gestual, escrita ou por aparelho eletrônico, salvo força maior autorizada pela Direção." },
  { topic:"Contato com a bancada antes", art:"Art. 21", keywords:"contato bancada antes perguntas antecipadas acesso previo respostas prontas vazamento",
    answer:"Antes da Sabatina, a candidatura só fala com a produção e a Direção de Jornalismo — nunca com a bancada. Ninguém tem acesso prévio às perguntas, aos temas do sorteio ou às respostas preparadas pelo outro lado." },
  { topic:"Fotos e vídeo pela imprensa da campanha", art:"Art. 22", keywords:"fotografo flash tripé equipamento fotografico registro imagens",
    answer:"Os profissionais de mídia da campanha podem fotografar/filmar só nos locais indicados, sem flash, tripé ou equipamentos que atrapalhem a transmissão. Quem descumprir pode ser retirado do estúdio." },
  { topic:"Duração total e estrutura", art:"Art. 23 e 24", keywords:"duracao total quanto tempo dura estrutura etapas ordem do programa",
    answer:"Cada Sabatina dura 55 minutos no total: abertura, apresentação da bancada e das regras, apresentação da candidatura, considerações iniciais, bloco de perguntas, considerações finais e encerramento." },
  { topic:"Apresentação da candidatura", art:"Art. 25 e 26", keywords:"apresentacao candidato quem apresenta trajetoria partido coligacao",
    answer:"A apresentação é feita só pela equipe de jornalismo, com dados objetivos (nome, partido, coligação, trajetória) — sem pedido de voto, número eleitoral ou qualquer conteúdo promocional." },
  { topic:"Considerações iniciais", art:"Art. 27 e 28", keywords:"consideracoes iniciais tempo inicial 1 minuto e 30 segundos abertura da fala",
    answer:"A candidatura tem até 1 minuto e 30 segundos para uma fala inicial, antes de começar a contagem oficial dos 45 minutos. Não pode pedir voto nem citar número eleitoral nessa fala." },
  { topic:"Ordem das perguntas", art:"Art. 29", keywords:"ordem perguntas sequencia fala povo bancada sorteio jornalista convidado o que vem primeiro",
    answer:"A ordem obrigatória é: Fala Povo, pergunta da bancada, sorteio de dois temas com manifestação sobre cada um, pergunta do jornalista convidado, nova pergunta da bancada, novo Fala Povo, e depois perguntas alternadas da bancada até acabar o tempo." },
  { topic:"Tempo oficial (45 minutos)", art:"Art. 30 e 31", keywords:"tempo oficial 45 minutos quanto tempo total contagem quando comeca",
    answer:"O tempo oficial da Sabatina é de 45 minutos, contados a partir da declaração do apresentador, e inclui tanto as perguntas quanto as respostas. As considerações iniciais e finais não entram nessa conta." },
  { topic:"Tempo de resposta (3 minutos)", art:"Art. 32 e 33", keywords:"tempo de resposta 3 minutos quanto tempo para responder cronometro renunciado",
    answer:"Cada resposta tem no máximo 3 minutos, contados a partir do fim da pergunta. Se o candidato terminar antes, o tempo que sobrou é perdido — não pode ser usado depois." },
  { topic:"Repetir a pergunta", art:"Art. 34", keywords:"repetir pergunta nao entendi pedir de novo",
    answer:"A candidatura pode pedir para repetir a pergunta quando não entender; quem repete é o mesmo jornalista que perguntou, e o cronômetro de 3 minutos só começa depois da repetição." },
  { topic:"Cronômetro e avisos sonoros", art:"Art. 35 e 36", keywords:"cronometro tempo restante aviso sonoro 30 segundos sinal visual",
    answer:"O tempo é controlado por um cronômetro no retorno de vídeo do candidato, com aviso sonoro faltando 30 segundos e outro ao término dos 3 minutos." },
  { topic:"Microfone desligado", art:"Art. 37", keywords:"microfone desligado falando demais estourou o tempo cortado",
    answer:"Se o tempo de resposta acabar e o candidato continuar falando, o microfone é desligado imediatamente até a condução normal do programa ser retomada." },
  { topic:"Pergunta feita perto do fim", art:"Art. 38", keywords:"pergunta no final do tempo ultrapassar 45 minutos direito de resposta completa",
    answer:"Se uma pergunta começar antes do fim dos 45 minutos, o candidato tem direito aos 3 minutos completos de resposta, mesmo que isso passe do tempo oficial da Sabatina." },
  { topic:"Falha técnica", art:"Art. 39", keywords:"falha tecnica problema tecnico interrupcao pausa remarcar",
    answer:"Se houver falha técnica que prejudique a Sabatina, o Diretor do Programa e o Coordenador de Jornalismo podem pausar a contagem e retomar do ponto exato em que parou." },
  { topic:"Sai do ar no YouTube ou rádio", art:"Art. 40 e 41", keywords:"youtube fora do ar radio caiu problema de sinal continua",
    answer:"Se o YouTube sair do ar mas o rádio continuar (ou vice-versa), a Sabatina segue normalmente pela plataforma que ainda está funcionando." },
  { topic:"Falta de energia", art:"Art. 42", keywords:"falta de energia eletrica forca maior remarcar sabatina",
    answer:"Em caso de falta de energia ou força maior, a Salvador FM aguarda até 5 minutos; se não resolver, a Sabatina é remarcada e a candidatura é avisada oficialmente." },
  { topic:"Fala Povo", art:"Art. 44 a 50", keywords:"fala povo perguntas do publico populacao pergunta gravada bairros quantas perguntas",
    answer:"O Fala Povo são perguntas gravadas com moradores de diferentes bairros de Salvador, produzidas só pela equipe de jornalismo, sem interferência de campanhas. Cada candidatura responde a 2 perguntas do Fala Povo, e ninguém tem acesso a elas antes." },
  { topic:"Perguntas da bancada", art:"Art. 51 a 62", keywords:"perguntas bancada jornalistas quem escolhe pode mudar acesso previo replica treplica",
    answer:"As perguntas da bancada são feitas livremente pelos jornalistas da Salvador FM, sem aprovação prévia de ninguém, alternando entre os jornalistas. Não há réplica nem tréplica, mas a bancada pode usar a pergunta seguinte para checar uma informação duvidosa dada pelo candidato." },
  { topic:"Sorteio dos temas", art:"Art. 63 a 72", keywords:"sorteio temas urna quantos temas sorteia recusar tema trocar tema lista de temas",
    answer:"Cada candidatura sorteia 2 temas ao vivo, numa urna física, e se manifesta sobre cada um antes do próximo sorteio. Não é possível recusar, trocar ou pedir novo sorteio, e o tema sorteado não volta para a urna." },
  { topic:"Lista de temas possíveis", art:"Anexo III", keywords:"quais temas lista assuntos possiveis sorteio saude educacao seguranca emprego",
    answer:"Os temas possíveis incluem, entre outros: saúde, educação/ciência/tecnologia, segurança pública, geração de empregos, infraestrutura, agropecuária, combate à pobreza, meio ambiente, saneamento, turismo, cultura, esporte, políticas para mulheres, gestão fiscal e economia do mar." },
  { topic:"Jornalista convidado", art:"Art. 73 a 80", keywords:"jornalista convidado quem escolhe pergunta convidada identidade secreta censura",
    answer:"Cada Sabatina tem 1 jornalista convidado de fora da emissora, escolhido só pela Salvador FM, cuja identidade e pergunta não são reveladas antes. Não há censura prévia nem pergunta complementar." },
  { topic:"Material impresso", art:"Art. 82", keywords:"material impresso anotacoes papel folha pode consultar durante",
    answer:"O candidato pode consultar livremente papéis, anotações, relatórios e documentos impressos, mas não pode mostrá-los às câmeras como recurso visual." },
  { topic:"Celular e eletrônicos", art:"Art. 83", keywords:"celular telefone tablet notebook fone de ouvido computador eletronico proibido pode usar",
    answer:"Não é permitido usar nenhum equipamento eletrônico durante a Sabatina — celular, tablet, notebook, fone de ouvido ou similares. Eles precisam ficar guardados com a equipe da campanha." },
  { topic:"Broche, roupa e materiais de campanha", art:"Art. 84", keywords:"broche adesivo camiseta bandeira santinho panfleto cartaz mesa roupa numero eleitoral",
    answer:"É permitido só um broche ou adesivo discreto de identificação na roupa. Roupa com pedido de voto, número eleitoral ou slogan de campanha não é permitida, assim como bandeiras, santinhos, panfletos ou cartazes na mesa." },
  { topic:"Recursos audiovisuais na resposta", art:"Art. 85", keywords:"grafico foto imagem tela banner apresentacao slide mostrar durante resposta",
    answer:"Não é permitido usar telas, gráficos, fotos, banners ou qualquer apoio audiovisual para ilustrar as respostas durante a Sabatina." },
  { topic:"Citar dados e pesquisas", art:"Art. 86", keywords:"citar dados estatisticas pesquisa eleitoral pode mencionar numeros",
    answer:"O candidato pode citar dados, estatísticas e pesquisas públicas, desde que respeite a legislação eleitoral sobre registro e divulgação de pesquisas." },
  { topic:"Ofensas e acusações", art:"Art. 87 a 89", keywords:"ofender acusar crime sem prova desrespeitar jornalista atacar instituicoes justica eleitoral",
    answer:"Não é permitido acusar alguém de crime sem provas públicas, desacreditar sem fundamento a Justiça Eleitoral ou o processo democrático, nem ofender ou desrespeitar jornalistas e a equipe do programa." },
  { topic:"Conteúdo derivado (cortes, reportagens)", art:"Art. 92 a 99", keywords:"cortes trechos reportagens podcast usar depois conteudo derivado divulgar",
    answer:"A Salvador FM pode produzir cortes, reportagens e outros conteúdos a partir da Sabatina, sempre com critério jornalístico e tratamento equivalente entre as candidaturas, preservando o contexto original." },
  { topic:"Compartilhar a Sabatina", art:"Art. 95", keywords:"compartilhar candidatura pode postar cortar editar trecho redes sociais campanha",
    answer:"As candidaturas podem compartilhar a íntegra ou trechos da Sabatina em seus canais, mas é proibido editar de um jeito que mude o contexto, o sentido ou a ordem das falas." },
  { topic:"Pedir cópia da gravação", art:"Art. 96", keywords:"copia gravacao integra pedido solicitar video",
    answer:"A campanha pode pedir cópia da íntegra da Sabatina por e-mail oficial; a Salvador FM entrega, quando possível, em até 2 dias úteis." },
  { topic:"O que acontece se descumprir as regras", art:"Art. 100 a 106", keywords:"punicao penalidade descumprimento medidas advertencia retirada consequencia",
    answer:"Dependendo da gravidade, a Salvador FM pode aplicar advertência verbal, interromper a fala, desligar o microfone, desconsiderar o que foi dito fora do tempo, retirar materiais proibidos ou até retirar da emissora quem estiver descumprindo as regras." },
  { topic:"Mudança de regras por decisão judicial", art:"Art. 107 e 108", keywords:"decisao judicial justica eleitoral mudar regras depois alteracao",
    answer:"Se a Justiça Eleitoral determinar mudanças no regulamento depois de divulgado, a Salvador FM avisa todas as campanhas oficialmente e pode pedir uma nova assinatura de concordância." },
  { topic:"Termo de concordância", art:"Art. 111 e 112", keywords:"termo assinar concordancia autorizar imagem voz",
    answer:"Para participar, a candidatura assina um Termo de Ciência e Concordância, autorizando o uso de sua imagem e voz para fins jornalísticos e institucionais da Salvador FM." },
  { topic:"Canal oficial de comunicação", art:"Art. 114", keywords:"contato oficial como falar com a salvador fm canal comunicacao email whatsapp",
    answer:"Toda comunicação oficial entre a Salvador FM e as campanhas acontece pelos canais previamente informados por cada campanha — e-mail, WhatsApp ou outro meio formal combinado entre as partes." },
  { topic:"Cronograma das Sabatinas", art:"Anexo I", keywords:"cronograma datas horarios quando vai ser quando e minha sabatina",
    answer:"O cronograma oficial (datas, horários, ordem de participação) é elaborado pela Salvador FM depois do sorteio e divulgado a cada campanha pelos canais oficiais informados." },
];

// ---------- Utilidades de busca ----------
function normalize(str){
  return str
    .toLowerCase()
    .normalize("NFD").replace(/[\u0300-\u036f]/g,"")
    .replace(/[^a-z0-9\s]/g," ")
    .replace(/\s+/g," ")
    .trim();
}

const STOP = new Set(["a","o","as","os","de","da","do","das","dos","e","ou","que","na","no","nas","nos",
  "para","com","por","um","uma","se","eh","e","sera","pode","posso","tem","ha","como","qual","quais",
  "sobre","durante","antes","depois","tenho","meu","minha","isso","essa","este","esta","sabatina"]);

function tokens(str){
  return normalize(str).split(" ").filter(t => t.length>1 && !STOP.has(t));
}

function score(queryTokens, entry){
  const hay = normalize(entry.keywords + " " + entry.topic + " " + entry.answer);
  let s = 0;
  queryTokens.forEach(t=>{
    if(hay.includes(t)) s += 2;
    // partial/stem match
    else if(hay.split(" ").some(w => w.startsWith(t.slice(0,4)) && t.length>=4)) s += 1;
  });
  return s;
}

function render(list, queryRaw){
  const results = document.getElementById("results");
  const hint = document.getElementById("hint");
  results.innerHTML = "";
  if(list.length === 0){
    hint.style.display="none";
    results.innerHTML = `<div class="no-result">Não encontrei uma resposta direta para <b>“${queryRaw}”</b> na base resumida.<br>
    Tente palavras mais simples (ex: “celular”, “tempo de resposta”, “sorteio”) ou consulte o regulamento completo com a produção pelos canais oficiais (Art. 114).</div>`;
    return;
  }
  hint.style.display="none";
  list.slice(0,5).forEach(entry=>{
    const card = document.createElement("div");
    card.className = "card";
    card.innerHTML = `
      <div class="card-top">
        <span class="badge">${entry.art}</span>
        <span class="topic">${entry.topic}</span>
      </div>
      <div class="answer">${entry.answer}</div>
    `;
    results.appendChild(card);
  });
}

function runSearch(){
  const raw = document.getElementById("q").value.trim();
  if(!raw){ document.getElementById("results").innerHTML=""; document.getElementById("hint").style.display="block"; return; }
  const qTokens = tokens(raw);
  const scored = KB.map(e => ({ e, s: score(qTokens, e) }))
                   .filter(x => x.s > 0)
                   .sort((a,b)=> b.s - a.s)
                   .map(x => x.e);
  render(scored, raw);
}

document.getElementById("q").addEventListener("keydown", e=>{
  if(e.key === "Enter") runSearch();
});

// chips de temas rápidos
const CHIP_TOPICS = ["Celular e eletrônicos","Tempo de resposta (3 minutos)","Sorteio dos temas","Fala Povo","Perguntas da bancada","Se o candidato faltar","O que acontece se descumprir as regras"];
const chipsEl = document.getElementById("chips");
CHIP_TOPICS.forEach(t=>{
  const b = document.createElement("button");
  b.className="chip"; b.type="button"; b.textContent=t;
  b.onclick = ()=>{ document.getElementById("q").value = t; runSearch(); window.scrollTo({top:280,behavior:"smooth"}); };
  chipsEl.appendChild(b);
});
</script>
</body>
</html>
