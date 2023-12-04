---
# Leave the homepage title empty to use the site title
title:
date: 2023-02-17
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:

  - block: collection
    id: posts
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 2
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'

  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Scientist - Machine Learning
          company: Meta Platforms, Inc
          company_url: 'www.meta.com'
          company_logo: meta
          location: New York, NY
          date_start: '2023-12-01'
          date_end:
          description: Recommendation System in Instagram
        - title: Post-doc Fellow
          company: Georgia Institute of Technology
          company_url: 'www.gatech.edu'
          company_logo: gt_vertical
          location: Atlanta, GA
          date_start: '2023-02-01'
          date_end: '2023-12-01'
          description: Bioinformatics and machine learning analysis of rNMP incorporation in DNA
        - title: Research Scientist Intern
          company: Norvatis
          company_url: 'www.novartis.com.cn'
          company_logo: norvatis
          location: Shanghai, China
          date_start: '2016-08-01'
          date_end: '2016-09-01'
    design:
      columns: '2'

  - block: portfolio
    id: projects
    content:
      title: Research
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # # Filter toolbar (optional).
      # # Add or remove as many filters (`filter_button` instances) as you like.
      # # To show all items, set `tag` to "*".
      # # To filter by a specific tag, set `tag` to an existing tag name.
      # # To remove the toolbar, delete the entire `filter_button` block.
      # buttons:
      #   - name: All
      #     tag: '*'
      #   - name: rNMPs
      #     tag: rNMPs
      #   - name: Software
      #     tag: Software
      #   - name: Other
      #     tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

 
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'

  - block: collection
    id: featured
    content:
      title: Recent Publications
      filters:
        folders:
          - publication
        featured_only: true
      count: 3
    design:
      columns: '2'
      view: list

  - block: accomplishments
    id: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url:
          date_end: ''
          date_start: '2023-01-31'
          description: ''
          organization: Keystone Symposia, USA
          organization_url: https://www.keystonesymposia.org/
          title: Future of Science Fund scholarship
          url: ''
        - certificate_url: https://bioinformatics.gatech.edu/congratulations-outstanding-bioinformatics-students
          date_end: ''
          date_start: '2022-05-01'
          description: 
          organization: Georgia Tech
          organization_url:
          title:  Mark Borodovsky Prize in the College of Sciences
          url: https://bioinformatics.gatech.edu/georgia-tech-couple-funds-prize-bioinformatics
        - certificate_url: 'https://research.gatech.edu/2022-suddath-award-winners'
          date_end:
          date_start: '2022-01-01'
          description: ''
          organization: Georgia Tech
          organization_url: 
          title: 2nd place in The F.L. "Bud" Suddath Memorial Award
          url: ''
        - certificate_url: ''
          date_end:
          date_start: '2022-01-01'
          description: ''
          organization: SERYM 2022
          organization_url: 
          title: Recogniation of outstanding contribution
          url: ''
        - certificate_url: ''
          date_end:
          date_start: '2021-01-01'
          description: ''
          organization: RNA 2021, 26th annual meeting of RNA society
          organization_url: 
          title: NSF Conference Award
          url: ''
    design:
      columns: '2'
 
  - block: collection
    id: talks
    content:
      title: Upcoming and Recent Presentations
      filters:
        folders:
          - event
      count: 3
    design:
      columns: '2'
      view: compact

  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'

  - block: features
    content:
      title: Skills and Hobbies
      items:
        - name: Machine Learning
          icon: chart-line
          icon_pack: fas
        - name: Deep Learning
          icon: circle-nodes
          icon_pack: fas
        - name: Bioinformatics
          icon: dna
          icon_pack: fas
        - name: Boardgame
          icon: chess-board
          icon_pack: fas
        - name: Hunting
          icon: paw
          icon_pack: fas
        - name: Tennis
          icon: person-running
          icon_pack: fas

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Let me know if you have any comments, questions, collaborative ideas, or just want to say hello!
      # Contact (add or remove contact options as necessary)
      email: xph6113@gmail.com
      phone: (+1) 706-765-9468
      # appointment_url: 'https://calendly.com'
      address:
        street: 770 Broadway
        city: New York
        region: NY
        postcode: '10003'
        country: United States
        country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
        # - 'Monday 10:00 to 13:00'
        # - 'Wednesday 09:00 to 10:00'
      contact_links:
       # - icon: video
        #  icon_pack: fas
        #  name: Contact me on Microsoft Teams
        #  link: 'https://teams.microsoft.com/l/chat/0/0?users=pxu64@gatech.edu'
        - icon: weixin
          icon_pack: fab
          name: xph56781234
      coordinates:
          latitude: '40.7310'
          longitude: '-73.9917'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: formspree
        formspree:
          id: 'xjvdwbqk'
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
    design:
      columns: '2'
---
