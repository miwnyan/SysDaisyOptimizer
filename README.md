---

# 🌼 SysDaisy Optimizer

> **Otimizador profundo para Windows com visual delicado e desempenho real.**
> Uma ferramenta completa de otimização, limpeza e ajustes avançados — com tema de margarida, interface confortável e foco em **desempenho real**, não em promessas vazias.

---

## 📖 Sobre o Projeto

O **SysDaisy Optimizer** é um otimizador para Windows criado em **PowerShell + WinForms**, pensado para entregar **otimizações profundas e reais** em três níveis de performance — sem interface poluída, sem enrolação e sem telemetria.

O visual é inspirado em uma **margarida**: tons escuros confortáveis para os olhos, com amarelo e verde suave como destaque. A ideia é simples: **cuidar do seu PC deve ser leve e agradável**.

---

## ✨ Recursos

### 🌼 Nível 1 — Performance Estruturada
- **Auto Tune** — aplica automaticamente as melhores otimizações (perfis Geral ou Gamer)
- **Deep Clean** — remove temporários, prefetch, cache do Windows Update e DNS
- **Disk I-O Boost** — TRIM em SSD e desfragmentação inteligente em HDD (multi-drive)

### 🌸 Nível 2 — Performance Avançada
- **Fix Low FPS** — encerra processos em segundo plano e desativa Game DVR
- **Boot Optimize** — ajusta o BCD para boot mais rápido
- **Fix FPS Drops** — estabiliza FPS com ajustes de CPU e rede
- **System Repair** — executа SFC + DISM para reparar arquivos corrompidos
- **Power Lock** — força o plano de energia *Alto Desempenho*
- **Shader Cache Reset** — limpa caches de shaders (NVIDIA, AMD e DirectX)
- **Pre-Game Clean** — limpeza rápida antes de jogar
- **Temp Clean** e **AppData Cache Clean** — limpezas seguras

### 🌻 Nível 3 — Performance Extrema
- **Kernel Tweak** — ajusta prioridades do kernel para resposta imediata
- **Debloat Services** — desativa serviços inúteis (telemetria, Xbox, SysMain, WSearch)
- **RAM Optimize** — otimiza alocação de memória e paginação
- **Driver Cache Clean** — limpa caches de drivers gráficos (fix stuttering)
- **Disable Visual FX** — remove animações e efeitos visuais
- **Deep System Clean** — limpeza profunda de logs e caches
- **Game Profile** — perfil extremo com ajustes de rede e sistema
- **Hibernation Killer** — desativa hibernação e remove o `hiberfil.sys`
- **Reserved Storage Fix** — libera espaço reservado do Windows
- **Registry Tweak** — ajustes avançados de registro **com backup automático**

---

## 🛡️ Segurança e Confiabilidade

- ✅ **Criação de ponto de restauração** com um clique
- ✅ **Backup automático do registro** antes de qualquer ajuste crítico
- ✅ **Logs detalhados** de cada operação (caminhos acessados, comandos executados, registros alterados)
- ✅ **100% reversível** — todas as modificações podem ser desfeitas
- ✅ **Sem telemetria** — nenhuma informação sai do seu computador

---

## 📂 Estrutura de Logs

Todos os registros ficam salvos localmente em:

```
%APPDATA%\SysDaisyOptimizer\
├── Logs\      # Histórico de todas as operações
├── Backups\   # Backups de registro (.reg)
├── Reports\   # Relatórios futuros
└── TermoDeUso.txt
```

Cada log contém:
- **Caminhos acessados** durante a operação
- **Comandos executados** com contexto
- **Registros alterados** com valores anteriores e novos
- **Status** (Sucesso / Erro) de cada ação

---

## 🖥️ Requisitos

- **Windows 10** ou **Windows 11** (x64)
- **PowerShell 5.1** ou superior
- Permissões de **administrador** (solicitadas automaticamente ao iniciar)

---

## 🚀 Instalação

### Opção 1 — Baixar o executável (recomendado)
1. Baixe o **`SysDaisyOptimizer.exe`** na aba [Releases](https://github.com/miwnyan/SysDaisyOptimizer/releases)
2. Coloque o `sysdaisyicon.ico` na mesma pasta (opcional — para o ícone da janela)
3. Execute. O UAC será solicitado automaticamente.

### Opção 2 — Rodar direto do script
```powershell
git clone https://github.com/miwnyan/SysDaisyOptimizer.git
cd SysDaisyOptimizer
powershell -ExecutionPolicy Bypass -File .\sysdaisy.ps1
```

### Opção 3 — Compilar você mesmo
```powershell
Install-Module -Name ps2exe -Force
Invoke-PS2EXE .\sysdaisy.ps1 .\SysDaisyOptimizer.exe `
    -iconFile .\sysdaisyicon.ico `
    -noConsole `
    -title "SysDaisy Optimizer" `
    -version "1.0.0.0"
```

---

## 🎨 Tema Visual

O SysDaisy usa uma paleta inspirada em uma margarida:

| Elemento | Cor | Hex |
|----------|-----|-----|
| Fundo | Oliva escuro | `#1A1C17` |
| Painéis | Verde-acinzentado | `#22241E` |
| Botões | Cinza-oliva | `#2B2E26` |
| Destaque | Amarelo margarida | `#FFD93D` |
| Texto | Creme quente | `#F5F0E0` |
| Acento verde | Verde folha | `#A8D5A2` |
| Detalhes | Rosa suave | `#FF9DC4` |

---

## ⚠️ Aviso

Este software realiza **modificações profundas no sistema operacional**. Ao utilizá-lo, você concorda que:

1. O uso é de **sua total responsabilidade**.
2. Recomenda-se **criar um ponto de restauração** antes de qualquer alteração (há um botão dedicado para isso).
3. Todas as modificações são reversíveis, mas podem exigir conhecimento técnico para desfazer manualmente.
4. O autor **não se responsabiliza** por eventuais danos causados pelo uso indevido.

---

## 🤝 Contribuindo

Contribuições são muito bem-vindas! Se você:

- 🐛 Encontrou um bug → abra uma [issue](https://github.com/miwnyan/SysDaisyOptimizer/issues)
- 💡 Tem uma sugestão → abra uma [discussion](https://github.com/miwnyan/SysDaisyOptimizer/discussions)
- 🔧 Quer contribuir com código → envie um **pull request**

Por favor, mantenha o padrão de código e o tema visual do projeto.

---

## 📜 Licença

Distribuído sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👤 Autor

**miwnyan**
- GitHub: [@miwnyan](https://github.com/miwnyan)

---

<div align="center">

**🌼 Feito com carinho para deixar seu Windows mais rápido. 🌼**

Se este projeto te ajudou, considere dar uma ⭐ no repositório!

</div>

---
---
- 📝 Um **CHANGELOG.md** inicial
- 🤝 Um **CONTRIBUTING.md**
- ⚙️ Um **template de Issue** para bugs

É só avisar! 🌼
