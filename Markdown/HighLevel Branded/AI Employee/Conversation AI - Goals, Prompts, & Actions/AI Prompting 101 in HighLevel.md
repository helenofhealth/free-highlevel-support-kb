**Date Updated:** 2024-04-11T21:13:36.000Z

You can achieve a lot with simple prompts, but the quality of results depends on how much information you provide it and how well-crafted the prompt is. A simple prompt can make your bot act as a bot, but a bot with a good prompt can vastly increase your human agency, build relationships and drive up business. 

  
**IN THIS ARTICLE**

* [Prompt Elements](#Prompt-Elements)
* [Best Prompting Practices](#Best-Prompting-Practices)
* [Elements in action](#Elements-in-action)  
   * [Role; specifying Interaction and Flow](#Role;-specifying-Interaction-and-Flow)  
   * [Task; specifying Instructions and Objectives](#Task;-specifying-Instructions-and-Objectives)  
   * [Guidelines; Guardrails for the bot to abide by ](#Guidelines;-Guardrails-for-the-bot-to-abide-by%C2%A0)
* [Best Practices in action](#Best-Practices-in-action)  
   * [Repetition](#Repetition)  
   * [Examples/Illustrations ](#Examples/Illustrations%C2%A0)
* [Advanced Prompting: ](#Advanced-Prompting%3A%C2%A0)  
   * [Delimiters ](#Delimiters%C2%A0)  
   * [Conversation Context ](#Conversation-Context%C2%A0)  
   * [Writing styles ](#Writing-styles%C2%A0)  
   * [Tone](#Tone)

  
## Prompt Elements

As we cover more and more examples and applications with prompt engineering, you will notice that certain elements make up a prompt. You can use these elements to instruct the model more effectively to improve the quality of results.

* Role; specifying Interaction and Flow \- persona, directions and context that can steer the AI model to better responses. Defining the role plays a pivotal part in the coherence and relevance of AI responses.
* Task; specifying Instructions and Objectives \- a specific task or instruction you want the model to perform, At the core of any successful prompt lies a well-defined task. Vague or ambiguous prompts might lead to your GPT bot hallucinating, or simply producing an outcome that’s not what you were expecting or which doesn’t meet your expectations.
* Guidelines; guardrails for bot to abide by \- guidelines are more like guardrails, steering the ChatBot toward desired outcomes. Clearly articulate rules to create a roadmap for more precise and tailored responses.

## Best Prompting Practices

* Repetition \- Incorporating repetition is key when you want to emphasize specific instructions, guiding the AI to respond more consistently in the desired direction. By reiterating critical parts of the prompt, you ensure the model's outputs align more predictably with your expectations. This approach is particularly effective in reinforcing the bot's adherence to essential guidelines or tasks.
* Examples/Illustrations \- Examples help AI ChatBots understand exactly what and how to do the required task, usually when describing the task is harder than just providing examples. Utilizing examples can significantly enhance an AI ChatBot's comprehension of the task at hand. While offering overarching instructions that span across all scenarios and permutations can be helpful, sometimes it's simpler to provide specific examples. This is particularly useful when aiming for the model to replicate a certain response style, tone or manner to user inquiries that are not easily described in words.
* Iterative Improvement \- While there are valuable tips and strategies for crafting prompts, developing effective ones for a GPT chatbot is fundamentally an iterative process. So before you set it out in the wild, you should test, tweak and fine-tune it as needed. Experimentation with various phrasings and methods is key to identifying what resonates best with your bot's objectives. Identifying the impact of modifications, such as new instructions or designs, can sometimes be challenging. Initial observations may provide some insights, yet small sample sizes might blur the distinction between genuine improvement and mere chance. To navigate this, use Bot Trial under ConversationAI to test, iterate and enhance your prompts and make the bot behave exactly as you want. The more you repeat this process, the better outcome your chatbot will achieve, and the better you will become at writing effective prompts

## Elements in action

### Role; specifying Interaction and Flow

* Worse:  
“You are a salesperson for {{ai.business\_name}}, assist customers and help them book appointments. Act like a human. You are talking to {{contact.name}}."
* Better:  
“- You work for {{ai.business\_name}}, your goal is to assist customers, qualify them on the basis of the answers they give to the questions you ask from the Script, and if qualified, you help them book appointments.  
\- Always maintain the persona of a human assistant. Do not disclose, suggest, or hint at being an AI assistant unless asked. Use colloquial language and phrases like "Great," "Got it," or "Understood" instead of formal apologies or offers of help.  
\- Acknowledge the user's input by repeating it back for clarity once at the start. After that, use varied affirmations or transitions without repeating the user's exact words.  
\- Maintain a professional, yet casual demeanor. Use periods instead of exclamation points to moderate the tone.  
\- You are talking to {{contact.name}}. Use the customer's first name only at the beginning and end of the conversation to avoid redundancy."

### Task; specifying Instructions and Objectives

* Worse:  
“You are required to qualify customers by asking them questions then asking them to book an appointment. If they are not interested, just collect their details.”
* Better:  
“Script Flow:  
\- Start by asking something like "What kind of marketing solution are you looking for?". If not interested, politely ask for their email and offer to stay in touch for future opportunities.  
\- If they have a positive response, ask "What telephony provider do you use for your marketing agency rn?".  
\- Once the customer has responded positively to all the asked questions through the conversation, only then propose scheduling a call with the team to discuss further.  
\- Before suggesting a booking, ask for their email address for booking the appointment if you do not already have it.  
\- Then help them book a call. Once booked, thank them and end the conversation on a positive note; looking forward to the scheduled call."

  
### Guidelines; Guardrails for the bot to abide by 

(You can specify these under Role and Instructions as well)

* Worse:  
"Reply in a concise manner. Ask all the questions in script and then have them book an appointment.”
* Better:  
“- Keep answers short, direct, and within a 20-word limit.  
\- Always wait for the user's response before asking the next question from the Script.  
\- Only have them book an appointment if they respond positively to the Script questions.”
  
  
## Best Practices in action

* ### Repetition

As we want our bot to follow the sales script we have put in place, we’d repeat/reference it multiple times.

* In Role we have:  
“- You work for {{ai.business\_name}}, your goal is to assist customers, qualify them on the basis of the answers they give to the questions you ask from the Script, and if qualified, you help them book an appointment.”
* In Guidelines we have:  
“- Always wait for the user's response before asking the next question from the Script.  
\- Only have them book an appointment if they respond positively to the Script questions.”
* ### Examples/Illustrations
* In Role we have:  
“- Always maintain the persona of a human assistant. Do not disclose, suggest, or hint at being an AI assistant unless asked. Use colloquial language and phrases like "Great," "Got it," or "Understood" instead of formal apologies or offers of help.”
* It can also be written as:  
“EXAMPLES OF WHAT TO SAY AND WHAT NOT TO SAY:

\- Avoid: I didn't understand your response.

\- Use: Wait, what did you say? Sorry, could you repeat that?

\- Avoid: I apologize for the confusion.

\- Use: Sorry if that didn't make sense.

\- Avoid: I understand your concern but I assure you our team is made up of highly trained professionals.

\- Use: Yeah, it makes sense why you'd be concerned but trust me, our team is really good at what we do.”
  
  
## Advanced Prompting: 

As we want our bot to follow the sales script we have put in place, we’d repeat/reference it multiple times.

* Static Information

You can add context or information about your business, offers, services in the prompt itself if you want the bot to have access to it all the time. It is recommended to keep the context under 100-200 words, as when the context size increases compared to the rest of the prompt, the prompt’s importance decreases for the AI ChatBot, as more of it is now around the context and not the prompt instructions.

* ### Delimiters

These are special characters you would use to emphasise or demarcate certain pieces of text (e.g. Context) in the prompt from other instructions in the prompt. 

* For emphasis you can use; #, >, <
* For demarcation you can use: “””, ‘’’, <> </>
* Example: Say you want to add some information about your offer in the prompt;  
Worse:  
“Offer: Elevate Your Business with Cutting-Edge A.I. Chatbots  
Transform the way you engage with your audience with our state-of-the-art A.I. chatbots, trusted by leading industry giants. Unlock the potential to skyrocket your lead generation, turbocharge sales, and redefine customer support, all while streamlining your operations.  
Imagine capturing not just any leads, but premium, one-click email opt-ins that elevate your marketing game. Dream of automating your sales process to generate revenue around the clock. Our technology refines targeting, significantly reducing lead acquisition costs and boosting conversion rates.  
But why stop there? Establish yourself as an authoritative figure in your niche by leveraging the unmatched efficiency and effectiveness of our bots. Whether it's your main venture or a lucrative side project, diving into the world of A.I. Chatbots opens up a realm of possibilities. Don't miss out on this trend—save time, dominate your market, and step into the future now.”  
Better:  
“# Offer:  
<offer>  
Elevate Your Business with Cutting-Edge A.I. Chatbots  
Transform the way you engage with your audience with our state-of-the-art A.I. chatbots, trusted by leading industry giants. Unlock the potential to skyrocket your lead generation, turbocharge sales, and redefine customer support, all while streamlining your operations.  
Imagine capturing not just any leads, but premium, one-click email opt-ins that elevate your marketing game. Dream of automating your sales process to generate revenue around the clock. Our technology refines targeting, significantly reducing lead acquisition costs and boosting conversion rates.  
But why stop there? Establish yourself as an authoritative figure in your niche by leveraging the unmatched efficiency and effectiveness of our bots. Whether it's your main venture or a lucrative side project, diving into the world of A.I. Chatbots opens up a realm of possibilities. Don't miss out on this trend—save time, dominate your market, and step into the future now.  
</offer>  
“
* ### Conversation Context

For specific use cases you can also add conversation context in the prompt, describing why and under what situation is the bot talking to a customer. You can start by setting the scene for the conversation; this will allow the chatbot to understand the context and provide more accurate responses. Just think about exactly what you want GPT to generate or achieve, and provide it with the prompt that’s most likely to get there. 

* Example, you can open the prompt by telling the chatbot why someone is interacting with it and what to do in the situation:  
Worse:  
“You are required to take on the role of a customer support chatbot”  
Better:  
“a client is contacting us because something went wrong” — and then telling it its role in the situation — “you must act as a friendly agent in charge of collecting a clear idea of what went wrong with the order, you need to ask them.”
* ### Writing styles

Analytical, Conversational, Creative, Descriptive, Informative, Instructive, Persuasive, Satirical, Technical etc.

* ### Tone

Authoritative, Clinical, Confident, Empathetic, Formal, Friendly, Humorous Informal, Optimistic, Playful, Sarcastic, Serious, Sympathetic, Warm etc.

  