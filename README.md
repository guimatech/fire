# fire 🔥

Fogueira interativa, 100% client-side (HTML + CSS + JavaScript puro).
Sem build step, sem dependências — um único arquivo (`index.html`) pronto para
deploy estático.

## Tecnologia

- **Chamas**: shader fragment WebGL com ruído fractal (fbm) para o movimento
  orgânico do fogo, reagindo a vento e combustível em tempo real.
- **Fagulhas e fumaça**: partículas em Canvas 2D, com a fumaça nascendo acima
  da ponta real da chama para um efeito sutil e realista.
- **Cena**: céu estrelado, brilho ambiente, anel de pedras e toras cruzadas
  desenhados proceduralmente em Canvas 2D.
- **Som**: crepitar do fogo sintetizado via Web Audio API (sem arquivos de
  áudio externos).

## Interação

- Mova o mouse (ou arraste o dedo no celular) perto do fogo: o vento inclina
  as chamas na direção do ponteiro.
- Clique/toque na fogueira: sopra o fogo, gerando uma rajada de fagulhas.
- Botões: **Soprar**, **Lenha** (aumenta o combustível/chamas) e **Som**
  (liga/desliga o crepitar).

## Rodar localmente

Basta abrir `index.html` em um navegador, ou servir a pasta:

```bash
python3 -m http.server 8080
```

## Deploy na Vercel

Projeto 100% estático — nenhuma build é necessária.

1. Importe este repositório na Vercel.
2. Framework preset: **Other** (ou deixe em branco).
3. Build command: *(vazio)*. Output directory: *(raiz / `.`)*.
4. Deploy.
