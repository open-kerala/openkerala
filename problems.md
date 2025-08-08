---
layout: default
title: Problems
---

<div class="container py-5" style="margin-top: 76px;">
    <div class="text-center mb-5">
        <h1 class="display-4 fw-bold">🔍 Kerala Problems</h1>
        <p class="lead">Real problems that need open-source solutions</p>
        <a href="https://github.com/open-kerala/openkerala/issues/new?template=problem-submission.md" class="btn btn-success">
            Submit a Problem
        </a>
    </div>
    
    <div class="row">
        {% for problem in site.problems %}
        <div class="col-md-6 col-lg-4 mb-4">
            <div class="card h-100">
                <div class="card-body">
                    <h5 class="card-title">{{ problem.title }}</h5>
                    <p class="card-text">{{ problem.excerpt | strip_html | truncate: 120 }}</p>
                    
                    {% if problem.district %}
                    <p class="text-muted small">
                        <i class="fas fa-map-marker-alt"></i> {{ problem.district }}
                    </p>
                    {% endif %}
                    
                    {% if problem.urgency %}
                    <span class="badge bg-{{ problem.urgency == 'high' ? 'danger' : problem.urgency == 'medium' ? 'warning' : 'info' }}">
                        {{ problem.urgency | capitalize }} Priority
                    </span>
                    {% endif %}
                </div>
                <div class="card-footer">
                    <a href="{{ problem.url | relative_url }}" class="btn btn-outline-primary btn-sm">Read More</a>
                    {% if problem.related_project %}
                    <a href="{{ problem.related_project }}" class="btn btn-success btn-sm">View Solution</a>
                    {% endif %}
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
    
    {% if site.problems.size == 0 %}
    <div class="text-center py-5">
        <h3>No problems submitted yet!</h3>
        <p class="lead">Help us identify problems that need solving in Kerala.</p>
        <a href="https://github.com/open-kerala/openkerala/issues/new?template=problem-submission.md" class="btn btn-success">
            Submit First Problem
        </a>
    </div>
    {% endif %}
</div>