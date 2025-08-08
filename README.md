# 🌿 OpenKerala

**Build Kerala, in the open.**

[![Website](https://img.shields.io/badge/Website-open--kerala.github.io-green)](https://open-kerala.github.io/openkerala)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Stars](https://img.shields.io/github/stars/open-kerala/openkerala?style=social)](https://github.com/open-kerala/openkerala/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/open-kerala/openkerala)](https://github.com/open-kerala/openkerala/issues)

> An open-source public innovation movement focused on building real, usable solutions to Kerala's problems—in full transparency, collaboration, and inclusivity.

## 🚀 What is OpenKerala?

We're not just a community. We're a collective of **developers, designers, activists, students, teachers, and everyday citizens** coming together to turn local problems into open-source projects that anyone can contribute to, use, or improve.

### 🎯 Our Mission
- **🔓 Open**: All code, content, and data are free and accessible
- **🌍 Local First**: Every project designed for Kerala's reality
- **🔄 Reusable**: Build once, reuse across regions
- **🎯 Impact-Focused**: Only real, needed problems—not vanity apps
- **🧠 Inclusive**: No tech skill required to contribute

## 🧩 How It Works

1. **🔍 Identify Problems** → People submit real issues from their communities
2. **📋 Curate & Open** → We frame problems as open collaboration opportunities
3. **🛠️ Build Together** → Create solutions with tech and non-tech contributors
4. **🔄 Share Back** → Everything public, reusable, and forkable

## 🤝 Who Can Join?

| Role | How You Can Help |
|------|------------------|
| 🧑💻 **Developers & Designers** | Build solutions, create interfaces |
| 🎨 **Artists & Content Creators** | Design graphics, create content |
| 🗣️ **Translators** | Make solutions accessible in local languages |
| 📚 **Teachers & Students** | Share knowledge, test solutions |
| 🧑🌾 **Farmers & Workers** | Share real problems, test solutions |
| 🧭 **NGOs & Panchayat Members** | Connect communities, validate impact |
| 🏛️ **Government Units** | Provide context, scale solutions |
| 🛰️ **Researchers & Engineers** | Technical expertise, data analysis |

## 🚀 Quick Start

### For Contributors
```bash
# 1. Submit a problem
Go to: Issues → New Issue → Problem Submission

# 2. Propose a project
Go to: Issues → New Issue → Project Proposal

# 3. Join existing projects
Browse: Issues labeled "help-wanted"
```

### For Developers
```bash
# Clone the repository
git clone https://github.com/open-kerala/openkerala.git
cd openkerala

# Install Jekyll (for local development)
gem install bundler jekyll
bundle install

# Run locally
bundle exec jekyll serve
# Visit: http://localhost:4000/openkerala
```

## 📁 Project Structure

```
openkerala/
├── _config.yml          # Jekyll configuration
├── _layouts/            # Page templates
├── _includes/           # Reusable components
├── _projects/           # Project showcase (markdown)
├── _problems/           # Problem submissions (markdown)
├── assets/              # Images, icons, files
├── css/                 # Stylesheets
├── js/                  # JavaScript
├── index.html           # Homepage
├── about.md             # About page
├── projects.md          # Projects listing
├── problems.md          # Problems listing
└── contribute.md        # How to contribute
```

## 📝 Adding Content

### Add a New Problem
Create `_problems/your-problem.md`:
```yaml
---
title: "Problem Title"
district: "District Name"
category: "environment|education|transport|health"
urgency: "high|medium|low"
affected_population: "Number of people affected"
---

Problem description here...
```

### Add a New Project
Create `_projects/your-project.md`:
```yaml
---
title: "Project Title"
district: "District Name"
status: "active|completed|planning"
tech_stack: ["React", "Node.js"]
github: "https://github.com/..."
---

Project description here...
```

## 🌐 Deployment

### GitHub Pages (Current)
- **URL**: https://open-kerala.github.io/openkerala
- **Auto-deploys** from `main` branch
- **Free hosting** via GitHub Pages

### Custom Domain (Future)
When `openkerala.org` is purchased:
1. Add `CNAME` file with domain
2. Update `_config.yml` URL
3. Configure DNS A records

## 🤝 Contributing

### Ways to Contribute
- 🐛 **Report bugs** via [Issues](https://github.com/open-kerala/openkerala/issues)
- 💡 **Submit problems** via [Problem Template](https://github.com/open-kerala/openkerala/issues/new?template=problem-submission.md)
- 🚀 **Propose projects** via [Project Template](https://github.com/open-kerala/openkerala/issues/new?template=project-proposal.md)
- 💻 **Code contributions** via Pull Requests
- 📝 **Documentation** improvements
- 🎨 **Design** and UI/UX enhancements

### Development Workflow
1. Fork the repository
2. Create feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

Read our [Contributing Guidelines](CONTRIBUTING.md) for detailed instructions.

## 📋 Roadmap

- [x] **Phase 1**: Website launch with Jekyll
- [x] **Phase 1**: Community structure and guidelines
- [ ] **Phase 2**: Problem submission system
- [ ] **Phase 2**: First 5 active projects
- [ ] **Phase 3**: Mobile-friendly solutions
- [ ] **Phase 3**: Government partnerships

See our detailed [Roadmap](ROADMAP.md) for more information.

## 📊 Current Stats

- **Problems Identified**: 2 (Water scarcity, Rural internet)
- **Active Projects**: 1 (Rainwater harvesting tracker)
- **Contributors**: Growing community
- **Districts Covered**: Ernakulam, Wayanad

## 🔗 Links

- **Website**: https://open-kerala.github.io/openkerala
- **GitHub**: https://github.com/open-kerala/openkerala
- **Issues**: https://github.com/open-kerala/openkerala/issues
- **Discussions**: https://github.com/open-kerala/openkerala/discussions
- **Contributing**: [CONTRIBUTING.md](CONTRIBUTING.md)
- **Code of Conduct**: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 💬 Community

- **GitHub Discussions**: For general questions and ideas
- **Issues**: For bug reports and feature requests
- **Pull Requests**: For code contributions

---

**Made with ❤️ for Kerala by the OpenKerala community**

*"Building Kerala, one open-source solution at a time."*