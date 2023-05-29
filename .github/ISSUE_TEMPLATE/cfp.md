name: 💬 Call for Proposal
description: Propose a session for a Schrödinger Session
body:
  - type: markdown
    attributes:
      value: |
        # Guidelines

        Remember to respect the following things while presenting your talk

        - Respect the Code of Conduct
        - Use an inclusive language

        The sessions are streamed on YouTube, but the speaker should attend in place. If you have any question feel free to drop a few lines to our [Email](mailto:events@schrodinger-hat.it)
  - type: dropdown
    id: format
    attributes:
      label: Format
      description: Please select the format of your talk
      options:
        - Talk (30 minutes)
        - Lightning Talk (15 minutes)
        - Workshop (> 2 hours)
    validations:
      required: true
  - type: textarea
    id: description
    attributes:
      label: Description
      placeholder: Describe your Session
    validations:
      required: true
  - type: input
    id: slides
    attributes:
      label: Link to the slides
      description: The slides of your session
    validations:
      required: false
  - id: places
    type: checkboxes
    attributes:
      label: In which city you may available to travel in to perform a session?
      options:
        - label: Florence, Italy 🇮🇹
          required: false
        - label: Verona, Italy 🇮🇹
          required: false
        - label: Milan, Italy 🇮🇹
          required: false
        - label: Turin, Italy 🇮🇹
          required: false
        - label: Paris, France 🇫🇷
          required: false
        - label: Brussels, Belgium 🇧🇪
          required: false 
  - id: places
    id: first-timer
    attributes:
      label: Are you a first-timer speaker?
      description: Please select the format of your talk
      options:
        - Yes, it's my first talk
        - No, I have a few experiences already
        - No, I am an experienced speaker
      validations:
        required: true
  - type: markdown
    attributes:
      value: |
        # Contacts and Socials

        Please leave here your main contacts so we can contact you if we need something!

        Remember to activate your GitHub notifications on this issue in order to be notified!
  - type: input
    id: linkedin
    attributes:
      label: LinkedIn
      description: LinkedIn URL
    validations:
      required: false
  - type: input
    id: twitter
    attributes:
      label: Twitter
      description: Your Twitter Handle
    validations:
      required: false