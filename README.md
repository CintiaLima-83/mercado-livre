# Projeto de Otimização de Performance Web

Este repositório contém um projeto front-end otimizado com foco em **performance, acessibilidade, SEO e boas práticas**.  
A análise foi realizada utilizando **Chrome DevTools (Lighthouse)**.

---

## 📌 Descrição do Projeto
Clone do Mercado Livre desenvolvido em HTML, CSS e JavaScript.  
O objetivo foi aplicar melhorias de performance e experiência do usuário, garantindo carregamento rápido e estável.

---

## 🔎 Análise Inicial
- **Desempenho:** 98 
- **Acessibilidade:** 81  
- **Práticas recomendadas:** 100 
- **SEO:** 91

### Gargalos identificados
- Imagens pesadas e sem compressão.  
- CSS não utilizado (~14 KiB).  
- Proporção incorreta em imagens.  
- Imports desnecessários.  
- Scripts bloqueando renderização.  

---

## 🛠️ Melhorias Aplicadas
1. **Imagens**
   - Conversão para **WebP**.  
   - Uso de `srcset` e `sizes` para versões menores em mobile.  
   - Atributo `loading="lazy"` aplicado em todas as imagens.  

2. **HTML/CSS/JS**
   - Minificação dos arquivos.  
   - Remoção de trechos não utilizados.  
   - Ajuste de contraste em botões e footer.  

3. **Imports**
   - Uso apenas dos módulos necessários do Font Awesome.  

4. **Código**
   - Fixação de largura/altura em imagens para evitar **CLS**.  
   - Uso de `object-fit: cover` para manter proporção correta.  

---

## 📈 Reanálise Final
- **Desempenho:** 100  
- **Acessibilidade:** 100  
- **Práticas recomendadas:** 100  
- **SEO:** 100  

### Métricas
- **FCP:** 1,5s  
- **LCP:** 1,5s  
- **TBT:** 0ms  
- **CLS:** 0  
- **Speed Index:** 1,5s  

---

## 📊 Comparativo Antes/Depois
| Métrica              | Antes | Depois |
|----------------------|-------|--------|
| Desempenho           | 98    | 100    |
| Acessibilidade       | 81    | 100    |
| Práticas recomendadas| 100   | 100    |
| SEO                  | 91    | 100    |

### Prints
- Relatório inicial: `/docs/lighthouse-before.png`  
- Relatório otimizado: `/docs/lighthouse-after.png`  

---

## 📌 Conclusão
As melhorias que trouxeram maior impacto foram:  
- **Otimização de imagens** (redução de tamanho e melhora no LCP).  
- **CSS enxuto** (remoção de código não utilizado).  
- **Contraste corrigido** (acessibilidade 100).  
- **Fixação de proporção das imagens** (práticas recomendadas 100).  

O projeto agora apresenta **100 em todas as categorias do Lighthouse**, garantindo uma experiência de usuário rápida, acessível e estável.
