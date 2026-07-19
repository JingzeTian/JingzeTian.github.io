---
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: 简介
      username: admin
  - block: experience
    content:
      title: 经历
      date_format: Jan 2006
      items:
        - title: 博士生
          company:  Laboratory of Empirical Research for Future Interfaces ([ERFI lab](https://sweb.cityu.edu.hk/canliu/team.html)), CityU
          company_url: ''
          company_logo: org-CityU
          location: 中国香港
          date_start: '2024-09-01'
          date_end: ''
          description:  |2-
            导师为[刘灿教授](https://sweb.cityu.edu.hk/canliu/index.html)，研究面向内容创作的思维工具——将 AI 辅助语音输入与直接操作相结合的界面。近期成果包括 Orality（共同一作，CHI'26）与 EchoLadder（UIST'25）。
        - title: 研究助理
          company: Accessible & Pervasive User EXperience ([APEX](https://www.mingmingfan.com/lab/)) Group, [香港科技大学（广州）](https://www.hkust-gz.edu.cn/)
          company_url: ''
          company_logo: org-HKUST-GZ
          location: 中国广州
          date_start: '2023-05-29'
          date_end: '2023-09-23'
          description: |2-
              在[樊明明教授](https://www.mingmingfan.com/)指导下、[Dr. Franklin](https://franklin-li.com/)协助下，独立提出研究想法并以负责人身份完成：

              * 文献综述与研究方案
              * 被试招募
              * 实验实施与结果分析
              * 论文撰写与投稿（CHI'24）
    design:
      columns: '2'
  - block: collection
    id: featured
    content:
      title: 近期论文
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
      title: 项目
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
      title: 联系
      subtitle:
      email: jingztian2-c@my.cityu.edu.hk
      wechat: ChatTJZ
      address:
        street: 香港城市大学创意媒体学院，达康道 18 号
        city: 九龙塘
        region: 九龙
        postcode: '999077'
        country: 中国香港
   
      autolink: true
    design:
      columns: '2'
---
