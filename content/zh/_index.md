---
# 官網大門總控設定
title: C.W. Chang Lab 物理化學實驗室
type: landing # 告訴 Hugo 這是首頁，不是一般的文章

sections:
  # 1. 主持人介紹 (About Me)
  - block: about.biography
    content:
      user: admin # 對應到 content/zh/authors/admin/ 資料夾
    design:
      background:
        color: '#f8f9fa'

  # 2. 最新動態 (News)
  - block: collection
    id: news
    content:
      title: 最新動態
      subtitle: 實驗室的科研進度與消息
      filters:
        folders:
          - news # 對應到 content/zh/news/
    design:
      columns: '2'
      view: compact

  # 3. 論文著作 (Publications)
  - block: collection
    id: publications
    content:
      title: 論文清單
      filters:
        folders:
          - publications # 對應到 content/zh/publication/
    design:
      columns: '1'
      view: citation

  # 4. 研究團隊 (members)
  - block: people
    id: people
    content:
      title: 研究團隊
      user_groups:
        - Principal Investigators
        - Students
    design:
      show_interests: true

  # 5. 儀器介紹 (Equipments)
  - block: collection
    id: equipments
    content:
      title: 儀器設備
      filters:
        folders:
          - equipments # 對應到 content/zh/equipment/
    design:
      columns: '2'
      view: card
---

歡迎來到張景維博士的物理化學實驗室網站。我們致力於**碳量子點 (Carbon Quantum Dots)** 與**納米材料**的前沿研究，特別是探索其在光譜分析中的螢光淬滅機制。