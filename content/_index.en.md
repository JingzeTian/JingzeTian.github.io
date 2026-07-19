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
            Advised by [Prof. Can Liu](https://sweb.cityu.edu.hk/canliu/index.html), I research thinking tools for content creation — interfaces that combine AI-assisted speech input with direct manipulation. Recent outcomes include Orality (co-first author, CHI'26) and EchoLadder (UIST'25).
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
  - block: collection
    id: featured
    content:
      title: Recent Publications
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '1'
      view: Citation
  - block: collection
    id: projects
    content:
      title: Projects
      count: 0
      filters:
        folders:
          - project
    design:
      view: masonry
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      email: jingztian2-c@my.cityu.edu.hk
      wechat: ChatTJZ
      address:
        street: 18 Tat Hong Avenue, CMC, City University of Hong Kong
        city: Kowloon Tong
        region: Kowloon
        postcode: '999077'
        country: Hong Kong
   
      autolink: true
    design:
      columns: '2'
---
