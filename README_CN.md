# Bolt.new Fork by Cole Medin - oTToDev

此版本的Bolt.new（oTToDev）允许您为每个提示选择使用的LLM！目前，您可以使用OpenAI、Anthropic、Ollama、OpenRouter、Gemini、LMStudio、Mistral、xAI、HuggingFace、DeepSeek或Groq模型 - 并且可以轻松扩展以支持Vercel AI SDK支持的任何其他模型！请参阅以下说明以在本地运行并扩展以包含更多模型。

## 加入oTToDev社区！

https://thinktank.ottomator.ai

## 此Fork的请求添加 - 欢迎贡献！！

- ✅ OpenRouter集成 (@coleam00)
- ✅ Gemini集成 (@jonathands)
- ✅ 自动生成已下载的Ollama模型 (@yunatamos)
- ✅ 按提供商过滤模型 (@jasonm23)
- ✅ 将项目下载为ZIP (@fabwaseem)
- ✅ 改进`app\lib\.server\llm\prompts.ts`中的Bolt.new主提示 (@kofi-bhr)
- ✅ DeepSeek API集成 (@zenith110)
- ✅ Mistral API集成 (@ArulGandhi)
- ✅ "Open AI Like" API集成 (@ZerxZ)
- ✅ 将文件同步（单向同步）到本地文件夹 (@muzafferkadir)
- ✅ 使用Docker容器化应用程序以便于安装 (@aaronbolton)
- ✅ 直接将项目发布到GitHub (@goncaloalves)
- ✅ 在UI中输入API密钥 (@ali00209)
- ✅ xAI Grok Beta集成 (@milutinke)
- ✅ LM Studio集成 (@karrot0)
- ✅ HuggingFace集成 (@ahsan3219)
- ✅ Bolt终端以查看LLM运行命令的输出 (@thecodacus)
- ✅ 代码输出的流式传输 (@thecodacus)
- ✅ 将代码恢复到早期版本的能力 (@wonderwhy-er)
- ✅ Cohere集成 (@hasanraiyan)
- ✅ 动态模型最大令牌长度 (@hasanraiyan)
- ✅ 提示缓存 (@SujalXplores)
- ✅ **高优先级** - 将本地项目加载到应用程序中 (@wonderwhy-er)
- ⬜ **高优先级** - 几乎完成 - 将图像附加到提示 (@atrokhym)
- ⬜ **高优先级** - 防止Bolt频繁重写文件（文件锁定和差异）
- ⬜ **高优先级** - 为较小的LLM提供更好的提示（代码窗口有时无法启动）
- ⬜ **高优先级** - 在后台运行代理而不是单个模型调用
- ⬜ 移动设备友好
- ⬜ Together集成
- ⬜ Azure Open AI API集成
- ⬜ Perplexity集成
- ⬜ Vertex AI集成
- ⬜ 直接部署到Vercel/Netlify/其他类似平台
- ⬜ 更好的提示增强
- ⬜ 让LLM在MD文件中规划项目以获得更好的结果/透明度
- ⬜ VSCode集成与类似git的确认
- ⬜ 上传文档以获取知识 - UI设计模板、参考代码库的编码风格等
- ⬜ 语音提示

## Bolt.new：浏览器中的AI驱动全栈Web开发

Bolt.new是一个AI驱动的Web开发代理，允许您直接从浏览器中提示、运行、编辑和部署全栈应用程序 - 无需本地设置。如果您想使用Bolt开源代码库构建自己的AI驱动Web开发代理，[请点击此处开始！](./CONTRIBUTING.md)

## Bolt.new的不同之处

Claude、v0等非常出色 - 但您无法安装包、运行后端或编辑代码。这就是Bolt.new的独特之处：

- **浏览器中的全栈开发**：Bolt.new将尖端AI模型与由**StackBlitz的WebContainers**驱动的浏览器内开发环境集成。这使您可以：
  - 安装并运行npm工具和库（如Vite、Next.js等）
  - 运行Node.js服务器
  - 与第三方API交互
  - 从聊天中部署到生产环境
  - 通过URL分享您的工作

- **具有环境控制的AI**：与传统的开发环境不同，AI只能在代码生成中提供帮助，而Bolt.new赋予AI模型对整个环境的**完全控制**，包括文件系统、节点服务器、包管理器、终端和浏览器控制台。这使AI代理能够处理整个应用程序生命周期 - 从创建到部署。

无论您是经验丰富的开发人员、PM还是设计师，Bolt.new都能让您轻松构建生产级全栈应用程序。

对于有兴趣使用WebContainers构建自己的AI驱动开发工具的开发者，请查看此仓库中的开源Bolt代码库！

## 设置

许多用户是第一次从Github安装软件。如果您在安装过程中遇到任何问题，请使用上面的链接提交“问题”，或者欢迎通过fork、编辑说明并提交pull请求来增强此文档。

1. 从https://git-scm.com/downloads安装Git

2. 从https://nodejs.org/en/download/安装Node.js

安装完成后请注意安装程序的说明。

在所有操作系统上，Node.js的路径应自动添加到系统路径中。但如果您想确认，可以检查路径。在Windows上，您可以在系统中搜索“编辑系统环境变量”，进入系统属性后选择“环境变量...”，然后检查“Path”系统变量中是否有Node的路径。在Mac或Linux机器上，它会告诉您检查/usr/local/bin是否在$PATH中。要确定$PATH中是否包含usr/local/bin，请打开终端并运行：

```
echo $PATH
```

如果在输出中看到usr/local/bin，那么您已经准备好了。

3. 克隆仓库（如果尚未克隆），打开终端窗口（或具有管理员权限的CMD），然后输入以下内容：

```
git clone https://github.com/coleam00/bolt.new-any-llm.git
```

3. 将.env.example重命名为.env.local并添加您的LLM API密钥。在Mac上，您可以在“[您的名字]/bold.new-any-llm/.env.example”找到此文件。对于Windows和Linux，路径类似。

如果看不到上述文件，可能是因为您无法查看隐藏文件。在Mac上，打开终端窗口并输入以下命令。在Windows上，您将在文件资源管理器设置中看到隐藏文件选项。如果卡在这里，快速Google搜索将帮助您。

```
defaults write com.apple.finder AppleShowAllFiles YES
```

**注意**：您只需设置您想要使用的API密钥，Ollama不需要API密钥，因为它运行在您的本地计算机上：

在此处获取GROQ API密钥：https://console.groq.com/keys

按照以下说明获取Open AI API密钥：https://help.openai.com/en/articles/4936850-where-do-i-find-my-openai-api-key

在您的账户设置中获取Anthropic API密钥：https://console.anthropic.com/settings/keys

```
GROQ_API_KEY=XXX
OPENAI_API_KEY=XXX
ANTHROPIC_API_KEY=XXX
```

可选地，您可以设置调试级别：

```
VITE_LOG_LEVEL=debug
```

如果使用Ollama，请设置DEFAULT_NUM_CTX，以下示例使用8K上下文并在localhost端口11434上运行ollama：

```
OLLAMA_API_BASE_URL=http://localhost:11434
DEFAULT_NUM_CTX=8192
```

**重要**：切勿将您的`.env.local`文件提交到版本控制中。它已经包含在.gitignore中。

## 使用Docker运行

先决条件：

如上所述的Git和Node.js，以及Docker：https://www.docker.com/

### 1a. 使用辅助脚本

提供了NPM脚本以方便构建：

```bash
# 开发构建
npm run dockerbuild

# 生产构建
npm run dockerbuild:prod
```

### 1b. 直接使用Docker构建命令（替代使用NPM脚本）

如果您愿意，可以使用Docker的目标功能来指定构建环境，而不是使用NPM脚本：

```bash
# 开发构建
docker build . --target bolt-ai-development

# 生产构建
docker build . --target bolt-ai-production
```

### 2. 使用Docker Compose配置文件运行容器

使用Docker Compose配置文件管理不同环境：

```bash
# 开发环境
docker-compose --profile development up

# 生产环境
docker-compose --profile production up
```

当您使用开发配置文件运行Docker Compose命令时，您对代码所做的任何更改将自动反映在容器中运行的站点上（即热重载仍然适用！）。

## 不使用Docker运行

1. 使用终端（或在Windows中使用具有管理员权限的CMD）安装依赖项：

```
pnpm install
```

如果收到“command not found: pnpm”或类似的错误，则意味着pnpm未安装。您可以通过以下方式安装它：

```
sudo npm install -g pnpm
```

2. 使用以下命令启动应用程序：

```bash
pnpm run dev
```

## 添加新的LLM：

要使新的LLM在此版本的Bolt.new中可用，请转到`app/utils/constants.ts`并找到常量MODEL_LIST。此数组中的每个元素都是一个对象，其中包含模型的ID（从提供商的API文档中获取）、前端模型下拉列表的标签以及提供商。

默认情况下，Anthropic、OpenAI、Groq和Ollama已实现为提供商，但此仓库的YouTube视频介绍了如何扩展以支持更多提供商！

当您向MODEL_LIST数组添加新模型时，它将在您本地运行应用程序或重新加载时立即可用。对于Ollama模型，请确保在尝试在此处使用之前已安装模型！

## 可用脚本

- `pnpm run dev`：启动开发服务器。
- `pnpm run build`：构建项目。
- `pnpm run start`：使用Wrangler Pages在本地运行构建的应用程序。此脚本使用`bindings.sh`设置必要的绑定，因此您无需复制环境变量。
- `pnpm run preview`：构建项目并在本地启动，用于测试生产构建。请注意，HTTP流式传输目前无法与`wrangler pages dev`正常工作。
- `pnpm test`：使用Vitest运行测试套件。
- `pnpm run typecheck`：运行TypeScript类型检查。
- `pnpm run typegen`：使用Wrangler生成TypeScript类型。
- `pnpm run deploy`：构建项目并将其部署到Cloudflare Pages。

## 开发

要启动开发服务器：

```bash
pnpm run dev
```

这将启动Remix Vite开发服务器。如果您使用Chrome，则需要Google Chrome Canary才能在本地运行此程序！这是一个简单的安装，也是一个非常适合Web开发的浏览器。

## 常见问题

### 如何获得oTToDev的最佳结果？

- **明确您的技术栈**：如果您想使用特定的框架或库（如Astro、Tailwind、ShadCN或任何其他流行的JavaScript框架），请在初始提示中提及它们，以确保Bolt相应地搭建项目。

- **使用增强提示图标**：在发送提示之前，尝试点击“增强”图标，让AI模型帮助您优化提示，然后在提交之前编辑结果。

- **先搭建基础，然后添加功能**：在深入更高级的功能之前，请确保应用程序的基本结构已就位。这有助于oTToDev理解项目的基础，并确保在构建更高级功能之前所有内容都已正确连接。

- **批量处理简单指令**：通过将简单指令合并到一个消息中来节省时间。例如，您可以要求oTToDev更改配色方案、添加移动响应性并重新启动开发服务器，所有这些都在一次操作中完成，从而节省时间并显著减少API信用消耗。

### 如何为oTToDev做出贡献？

[请查看我们为oTToDev贡献的专用页面！](CONTRIBUTING.md)

### 您计划将oTToDev合并回官方的Bolt.new仓库吗？

更多消息将在下月初发布 - 敬请期待！

### oTToDev的未来计划是什么？

[在此查看我们的路线图！](https://roadmap.sh/r/ottodev-roadmap-2ovzo)

更多更新即将发布！

### 为什么有这么多未解决的问题/拉取请求？

oTToDev最初只是为了展示如何编辑开源项目，并在我的（@ColeMedin）YouTube频道上做一些与本地LLM相关的酷事！然而，它迅速成长为一个庞大的社区项目，我正在努力通过组建维护者团队并让尽可能多的人参与来满足需求。
这项努力进展顺利，我们所有的维护者都是绝对的摇滚明星，但仍然需要时间来组织一切，以便我们能够高效地处理所有问题和PR。但请放心，我们正在努力工作，甚至正在幕后进行一些合作，以真正帮助这个项目起飞！

### 本地LLM与Claude 3.5 Sonnet等大型模型相比，oTToDev/Bolt.new的表现如何？

尽管开源模型与大型闭源模型之间的差距正在迅速缩小，但您仍然会从GPT-4o、Claude 3.5 Sonnet和DeepSeek Coder V2 236b等非常大的模型中获得最佳结果。这是我们面临的一大任务 - 找出如何更好地提示、使用代理并改进平台整体，以使其更好地适用于较小的本地LLM！

### 我收到错误：“处理此请求时出错”

如果您在oTToDev中看到此错误，这只是应用程序告诉您存在高级别问题，这可能意味着许多不同的事情。要查找实际错误，请检查您启动应用程序的终端（使用Docker或pnpm）和浏览器中的开发者控制台。对于大多数浏览器，您可以通过按F12或右键单击浏览器中的任何位置并选择“检查”来访问开发者控制台。然后转到右上角的“控制台”选项卡。

### 我收到错误：“缺少x-api-key标头”

我们已经看到此错误几次，出于某种原因，只需重新启动Docker容器即可修复。这似乎是Ollama特定的问题。另一个尝试的方法是尝试使用Docker或pnpm运行oTToDev，无论您第一次没有运行哪个。我们仍在寻找为什么有时会发生这种情况的原因！

### 当oTToDev运行我的应用程序时，我得到一个空白预览！

我们向您保证，我们正在不断测试进入oTToDev的新PR，预览是核心功能，因此应用程序没有损坏！当您得到空白预览或没有得到预览时，这通常是因为LLM生成了错误的代码或错误的命令。我们正在努力使这一点更加透明，以便显而易见。有时错误也会出现在开发者控制台中，因此也请检查一下。

### 一切正常，但结果不好

这与上述关于本地LLM变得非常强大但您仍然会从最大的LLM（如GPT-4o、Claude 3.5 Sonnet和DeepSeek Coder V2 236b）中看到更好（有时甚至更好得多）的结果的观点有关。如果您使用的是较小的LLM（如Qwen-2.5-Coder），请将其视为更具实验性和教育性。它可以很好地构建较小的应用程序，这对于本地LLM来说非常令人印象深刻，但对于更大规模的应用程序，您仍然希望使用较大的LLM！