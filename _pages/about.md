---
permalink: /
title: ""
author_profile: true
redirect_from:
- /about/
- /about.html
---

<!-- 
{% include about/intro.md %} -->

<div id="about-page" class="accordion">

    <!-- Research Style -->
    <div class="card">
        <div class="card-header" id="headingResearchStyle" style="background-color: #333; color: #fff;">
            <h2 class="mb-0">
                <button class="btn btn-link category-btn collapsed" type="button" data-toggle="collapse"
                    data-target="#collapseResearchStyle" aria-expanded="false" aria-controls="collapseResearchStyle"
                    style="color: #fff;">
                    🎓 My Research Style
                </button>
            </h2>
        </div>
        <div id="collapseResearchStyle" class="collapse" aria-labelledby="headingResearchStyle"
            data-parent="#about-page">
            <div class="card-body" style="background-color: #f8f9fa; color: #000;">
                {% include about/research_style.md %}
            </div>
        </div>
    </div>

    <!-- Interests -->
    <div class="card">
        <div class="card-header" id="headingInterests" style="background-color: #333; color: #fff;">
            <h2 class="mb-0">
                <button class="btn btn-link category-btn collapsed" type="button" data-toggle="collapse"
                    data-target="#collapseInterests" aria-expanded="false" aria-controls="collapseInterests"
                    style="color: #fff;">
                    🔭 My Interests
                </button>
            </h2>
        </div>
        <div id="collapseInterests" class="collapse" aria-labelledby="headingInterests" data-parent="#about-page">
            <div class="card-body" style="background-color: #f8f9fa; color: #000;">
                {% include about/interests.md %}
            </div>
        </div>
    </div>

    <!-- On-going Projects -->
    <div class="card">
        <div class="card-header" id="headingProjects" style="background-color: #333; color: #fff;">
            <h2 class="mb-0">
                <button class="btn btn-link category-btn collapsed" type="button" data-toggle="collapse"
                    data-target="#collapseProjects" aria-expanded="false" aria-controls="collapseProjects"
                    style="color: #fff;">
                    🚀 On-going Projects
                </button>
            </h2>
        </div>
        <div id="collapseProjects" class="collapse" aria-labelledby="headingProjects" data-parent="#about-page">
            <div class="card-body" style="background-color: #f8f9fa; color: #000;">
                {% include about/ongoing_projects.md %}
            </div>
        </div>
    </div>

    <!-- Work Experience -->
    <div class="card">
        <div class="card-header" id="headingExperience" style="background-color: #333; color: #fff;">
            <h2 class="mb-0">
                <button class="btn btn-link category-btn collapsed" type="button" data-toggle="collapse"
                    data-target="#collapseExperience" aria-expanded="false" aria-controls="collapseExperience"
                    style="color: #fff;">
                    💼 Work Experience
                </button>
            </h2>
        </div>
        <div id="collapseExperience" class="collapse" aria-labelledby="headingExperience" data-parent="#about-page">
            <div class="card-body" style="background-color: #f8f9fa; color: #000;">
                {% include about/work_experience.md %}
            </div>
        </div>
    </div>

    <!-- Education -->
    <div class="card">
        <div class="card-header" id="headingEducation" style="background-color: #333; color: #fff;">
            <h2 class="mb-0">
                <button class="btn btn-link category-btn collapsed" type="button" data-toggle="collapse"
                    data-target="#collapseEducation" aria-expanded="false" aria-controls="collapseEducation"
                    style="color: #fff;">
                    🎓 Education
                </button>
            </h2>
        </div>
        <div id="collapseEducation" class="collapse" aria-labelledby="headingEducation" data-parent="#about-page">
            <div class="card-body" style="background-color: #f8f9fa; color: #000;">
                {% include about/education.md %}
            </div>
        </div>
    </div>

</div>