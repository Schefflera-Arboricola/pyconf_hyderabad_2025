**Disclaimer** : These note are for my reference; probably won't be understandable by everyone. Not written with general public in mind. Also everything in these might not be correct. These are rough notes.

- https://icodeschool.com/

- Keynote 1:
    - Writing python spec
    - Trainer, explainers, sustainers: what happen when LLMs can program themselves(trainers will go)
    - Linkedin Vs reality
    - 2 things in GPT: 
        - Predict next words/token
        - Find similarities between tokens based on what it has seen before
        - Markov chains (chandamama —> dor -> ke) —> like that library/canteen flow example(from coder’s high)
        - LLM doesn’t know python, it predicts
    - Markovian chain making website
    - Row-something diagrams
    - AI is good at problems that are already seen by it… struggles with 
    - def find_customer() —> predicts good, def f() —> terribly predicts
    - New API changes—> AI doesn’t know those, and those are not widely adapted
    - with open(input=“file.txt”, bananas=12): —> it will predict further code with `bananas` but later would tell this is wrong if asked what’s the error, but cannot connect the 2
    - Senior developers
        - Good tests
        - Using scalable patterns
        - Questions requirements and clarify designs before implementing (edge cases)
    - Python to AI —> going along the trend
    - AI can’t do:
        - AI can only handle little bits of data (paper : lost in the middle)
            - 128000 bits; recall rate drops if a lot of info is given---???
        - AI’s knowledge is generic and old - API changes
            - pydantic 2, numpy 2 —> fail
        - LLMs cannot do calculations
            - How do they calculate?
            - Can’t do math with prediction — not very accurate(rocket launching calculations!)
    - Test coverage… fuzzer, hypothesis(for improving test)
    - Making code fast: run profiler (Ask AI: reasons for the bottle-necks in a given code)
    - AI is good at:
        - Summarisations and QnA
        - Data driven decisioning - accessing reviews
        - Personalisation: translate(task) and my intension of doing this is xyz(give context) - informal and formal Japanese (emails’ , cover letters’ and SoPs’ polishing)
        - Automation: repetitive task (tomorrow’s workshop)
    - 
    - Making small changes: refactoring
    - Writing code: auto complete in code editors
    - Testing: don’t use AI initially, use it afterwards(listen to recording later)
    - Designing and solution: present this to my senior, creating diagrams
    - 
    - Detailed question —> detailed prompt —> good answer
        - Asking AI to write a prompt for itself, (and then improve it), and then give it back to AI, probably won’t consider edge cases, error messages 
    - Focus on problem solving (it’s “Artificial” Intelligence, write detailed specific prompts)
    - Development is kind of repetitive, AI can help with it
    - Supervise AI , use it as a helping hand, focus on the important stuff, write scalable and reliable code, limitations of AI
    - Confident answer != right answer
    - Problem solving skills, know what AI can do and cannot do…

    - What if we hard code the original sources or rules of maths, (domain specific LLMs), give more weights or priority to info by original source?



- PEP talk (pep numbers might not be right!)
    - Something is better than nothing — do it because it makes sense right now
    - Type-hints came in 2010? (PEP 3107) - pep 484
    - PEG parser expression grammer (PEP 617)
    - PEP 635 : match-case
    - PEP 703: GIL in CPython
    - Free-threaded python —> naming things(how people would use the words)


- Old laptop to home sever talk
    - Old laptop for storage
    - Debian - minimal , “arch install sudo” to install sudo
    - Passwordless ssh server
    - Jio -- free public ipv6 address
    - Proxied address
    - Reverse proxy engine


- Keynote 2:
    - Your financial situation is someone else's decision??
    - Frappe framework 
    - Supporting small businesses through open source 
    - Community, free (money, freedom) : open-source
    - School management using frappe 
    - Listmonk : self hosted newsletter?, Go lang, Vue js, postgres


- RAG talk:
    - Bulb - explain previous 2 slides
    - Knowlege based and search the web
    - Gargrils? - jail breaking prompt?
    - Outreach ai?
    - https://github.com/agno-agi/agno


- Feedback on dispatching talk(by me):
    - in-person feedback(not a qoute) : Explain entry_points with the same simple example of “library_1” “library_2”, instead of flashing all info about entry-point in one slide...
    - Me: 
        - keep in mind the time... maybe I can remove some things?
        - Don’t mention "mysterious" red cloud --> adds confusion
        - try and concentrate on(or say the word) "entry-point"(and/or "extend the functionality"(something people tend to think it's like a C extension) or "plug-in arch") more than dispatching/dispatchable --> otherwise people tend to conclude I'm talking about the "dispatcher" in a different sense I guess.
    - Anonymous from slido.com : "Great job aditi. Personally, i would have told the story in a different way but you conveyed the technical content well. Kudos on the work overall - it's great to see folks from India working on the scientific python ecosystem"


- workshop : AI-agents
    - https://github.com/marketplace/models/azure-openai/gpt-4o-mini/playground
    - Temperature : randomness, creativity, temperature is high then we get different things every time we run the same prompt
    - Delete chat history when you reset the prompt—> so that history is not used as context for new model
    - LLMs are limited, improve functionality using agents
    - Shopping website chatbot —> access login info and order history
    - pydantic ai, autogen, llm.., MagenticOneGroupChat, RoundRobinGroupChat
    - https://microsoft.github.io/autogen/0.2/docs/tutorial/introduction/ 
    - https://github.com/tonybaloney/autogen/blob/workshop/workshop/quickstart.ipynb 
    - max_turns=2 —> chat termination(terminate chat after 2 messages)
    - https://github.com/tonybaloney/autogen/tree/workshop
    - https://platform.openai.com/docs/guides/function-calling : using enum
