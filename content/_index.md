---
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      username: admin
  - block: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: PhD Student
          company:  Laboratory of Empirical Research for Future Interfaces ([ERFI lab](https://sweb.cityu.edu.hk/canliu/team.html)), CityU
          company_url: ''
          company_logo: org-CityU
          location: Hong Kong, China
          date_start: '2024-09-01'
          date_end: ''
          description:  |2-
            With the instruction of my supervisor Prof. Can, studied and investigated the affordance of Speech-to-text input.
        - title: Research Assistant
          company: Accessible & Pervasive User EXperience ([APEX](https://www.mingmingfan.com/lab/)) Group, [Hong Kong University of Science and Technology (Guangzhou)](https://www.hkust-gz.edu.cn/)
          company_url: ''
          company_logo: org-HKUST-GZ
          location: Guangzhou, China
          date_start: '2023-05-29'
          date_end: '2023-09-23'
          description: |2-
              With the instruction of [Prof. Mingming Fan](https://www.mingmingfan.com/) and the assistance of [Dr. Franklin](https://franklin-li.com/), independently generated a research idea and as a leader, accomplished the following tasks:

              * Literature review and Research protocol
              * Participants recruitment
              * Conducting experiments and results analysing
              * Paper writing and submission (CHI'24)
    design:
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      default_button_index: 0
      buttons:
        - name: All
          tag: '*'
        - name: Research
          tag: Research
        - name: Development
          tag: Development
        - name: Design
          tag: Design
    design:
      columns: '2'
      view: Masonry
      flip_alt_rows: false
  - block: collection
    content:
      title: Recent Publications
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '3'
      view: Citation
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      email: tianjingzetjz@163.com
      phone: +86 13919328307
      wechat: ChatTJZ
      address:
        street: Moling Street
        city: Jiangning District, Nanjing
        region: Jiangsu
        postcode: '211189'
        country: China
      autolink: true
    design:
      columns: '2'
---
