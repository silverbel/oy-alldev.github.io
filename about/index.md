---
layout: main
main: true
title: 개발팀 소개
---

<div class="loading-animation">
    <div class="about">
        <div class="section">
            <div class="title index">01</div>
            <div class="content">
                <h1 class="subtitle">개발문화</h1>
                <ul class="culture">
                    <li>모든 코드는 애정어린 리뷰를 거칩니다.</li>
                    <li>직관적이고 명확하거나 재기발랄한 네이밍을 추구합니다.</li>
                    <li>무엇을 목적으로 하는지, 어디로 가고자 하는지 충분히 고민하고 논의 합니다.</li>
                    <li>가급적 주석이 불필요한 코드를 만들어 냅니다.</li>
                    <li>개성은 존중하되, 조화로움을 중시 합니다.</li>
                    <li>야근을 한다면, 나를 위한 야근을 합니다.</li>
                    <li>일을 독점하지 않습니다. 나는 언제든 휴가를 떠날 수 있는 여행가입니다.</li>
                    <li>자기 발전에 노력을 아끼지 않고, 공유로 함께 성장할 수 있는 환경을 만듭니다.</li>
                    <li>장애를 잘 처리하는 팀 보다는, 장애가 없는 팀이 되도록 노력 합니다.</li>
                    <li>실패 보다 머무름을 두려워 합니다.</li>
                </ul>
            </div>
        </div>
        <div class="section">
            <div class="title index">02</div>
            <div class="content">
                <h1 class="subtitle">개발환경</h1>
                <ul class="environment">
                    <li>소스는 내부 GitLab 저장소를 사용해 관리하고 있습니다.</li>
                    <li>타팀과의 업무는 레드마인을 통해 관리/진행합니다.</li>
                    <li>개발팀 내부에서는 GitLab 이슈를 통해 업무에 대한 작업 내역을 관리합니다.</li>
                    <li>회사 내 커뮤니케이션은 Slack을 사용합니다.</li>
                    <li>문서는 위키를 사용해 작성합니다.</li>
                </ul>
            </div>
        </div>
        <div class="section">
            <div class="title index">03</div>
            <div class="content">
                <h1 class="subtitle">개발자 소개</h1>
                <div class="divider"></div>
                <div class="group">
                    <div class="group-name">#백엔드 #인프라 #웹</div>
                    <ul class="member">
                        {% assign members = site.data.members | where: 'group', 'backend' | sort: 'id' %}
                        {% for member in members %}
                            {% include about-member.html %}
                        {% endfor %}
                    </ul>
                </div>
                <div class="group">
                    <div class="group-name">#데이터 #DBA</div>
                    <ul class="member">
                        {% assign members = site.data.members | where: 'group', 'data' | sort: 'id' %}
                        {% for member in members %}
                            {% include about-member.html %}
                        {% endfor %}
                    </ul>
                </div>
                <div class="group">
                    <div class="group-name">#프론트엔드 #웹 #퍼블리셔</div>
                    <ul class="member">
                        {% assign members = site.data.members | where: 'group', 'frontend' | sort: 'id' %}
                        {% for member in members %}
                            {% include about-member.html %}
                        {% endfor %}
                    </ul>
                </div>
                <div class="group">
                    <div class="group-name">#앱 #Android #iOS</div>
                    <ul class="member">
                        {% assign members = site.data.members | where: 'group', 'app' | sort: 'id' %}
                        {% for member in members %}
                            {% include about-member.html %}
                        {% endfor %}
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>
