---
layout: default
title: Projects
---

<div class="container py-5" style="margin-top: 76px;">
    <div class="text-center mb-5">
        <h1 class="display-4 fw-bold">🧩 OpenKerala Projects</h1>
        <p class="lead">Real solutions for real problems</p>
    </div>
    
    <div class="row">
        {% for project in site.projects %}
        <div class="col-md-6 col-lg-4 mb-4">
            <div class="card project-card h-100">
                <div class="card-body">
                    <h5 class="card-title">{{ project.title }}</h5>
                    <p class="card-text">{{ project.excerpt | strip_html | truncate: 120 }}</p>
                    
                    {% if project.district %}
                    <p class="text-muted small">
                        <i class="fas fa-map-marker-alt"></i> {{ project.district }}
                    </p>
                    {% endif %}
                    
                    {% if project.status %}
                    <span class="badge bg-{{ project.status == 'active' ? 'success' : project.status == 'completed' ? 'primary' : 'secondary' }}">
                        {{ project.status | capitalize }}
                    </span>
                    {% endif %}
                </div>
                <div class="card-footer">
                    <a href="{{ project.url | relative_url }}" class="btn btn-outline-success btn-sm">Learn More</a>
                    {% if project.github %}
                    <a href="{{ project.github }}" class="btn btn-success btn-sm">
                        <i class="fab fa-github"></i> Code
                    </a>
                    {% endif %}
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
    
    {% if site.projects.size == 0 %}
    <div class="text-center py-5">
        <h3>No projects yet!</h3>
        <p class="lead">Be the first to contribute a project to OpenKerala.</p>
        <a href="https://github.com/open-kerala/openkerala/issues/new?template=project-proposal.md" class="btn btn-success">
            Propose a Project
        </a>
    </div>
    {% endif %}
</div>