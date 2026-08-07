# Transcript — Post-Sprint Planning and Technical Alignment Meeting

Meeting ID: meeting-643d090e-77a4-4185-b6d9-cabb0eb3ef1d
Date: 4 August 2026 (Week 3)
Source: auto-transcript, pasted by Johnson. Proper nouns are unreliable (e.g. "Wite" = Vite, "Super Bass" = Supabase, "Mango" = MongoDB, "spring" = sprint).

---

[00:00] I'll get up today and I'll share the link so that everyone will get the book. Yeah, sure.
[00:28] I feel like whips on the phone would be better since I think everyone's tech stack. Yeah. So I reckon React will be fine. Yeah. Cause we can easily transfer into a React native or literally you can just change the view based on the.
[01:03] Mongo or Super Bass? I think. Do you guys have any prefers? I've tried them both, so I don't mind.
[01:29] You guys have any preferred?
[01:31] That'll be easier for you.
[01:38] Let's do one for this one.
[01:44] I think React with Wite framework. Yeah, it should be alright.
[01:58] For the backend, you were thinking about Java. I was thinking of using Express, so Node.js.
[02:27] Java will be Spring Boot, right? Yeah, Java Spring Boot.
[02:33] database, mongodb and what the what? mongodb would be fine we can put up a code if you want something else we can put up a code I mean it's the same it will be sequel it will be basically yeah it will be postgres oh sorry it will be postgres in that case my will be yes superbased yeah
[02:57] could put yeah so mango and super bass and super bassing for the brackets a
[03:09] Yeah. And I think... And should we use Docker for... Yeah.
[03:28] Based on my experience, Docker will be easy, because the project I'm working on is using Docker.
[03:52] This is a healthcare robot, right? Healthcare robot related, so...
[03:59] It's like, it's a hard way, but we have to develop the software. But how we can demonstrate that? We have to check and get in detail. It's more like he become a robot and try for two different people and check the database and have the data. And then if Jamuna comes and see the records for that particular user, she's able to access all the history. And then on the table you have your normal schema and then user table joined with some sort of data on ID.
[04:38] So, something I was thinking was we could break it down to like small parts, so make it like, because they want to make it like generic, right? So, I was thinking of we should break down the table to like very small, finer tables. So, just say you have a user table, just the ID and the name, and then you have, let's say, the health data or whatever, the patient's data, just drawing, just using ID , because that's your ID, your unique identifier. and you can just join the two tables.
[05:18] Yeah In this case we are acting as a robot one from the different worlds. That's the base of the robot. It's a very basic website it looks like.
[06:04] like what we discussed before. Because in my brain, I was still thinking of...
[06:08] user base so like each user goes in and have like
[06:13] They have their own table, they have their own access.
[06:26] In the physical world robots are there and trying to maintain the medicine records for users.
[06:35] In that case, we as a creator or a user are robots and some third person is our patient. Let's use two words, patient and the users. Users are basically the robots which we are and the patients are for which the data is being used. If that makes sense. Is that correct? So basically making a website is just for like a demo purpose. Exactly. A robot doesn't need a UI. That's what I'm saying. They just need an API in two points. So the robots will be accessing all the API calls. Robots are basically your mobile.
[07:23] More or less if you talk about because they have everything scored once they go to a particular person they will scan the face and they will get the idea.
[07:31] So if it is something like some data, the person has to take medicine, it has to send a notification something. don't do data erasers, not two robots changing one mind.
[08:07] If that makes sense. So for example, a person needs to take two types of medicines, medicine A and medicine B. And robot one going in, they just feed him the medicine A, and then it clicked save, but at the exact same time that robot two came in, oh, it sees this person hasn't taken medicine A, it gives medicine out again. So I think that's the only thing we need to think about. Ah, okay. Yeah. I mean, I think
[09:11] Yeah, but you still have to think about the problem where I mean we can discuss this later, but this is a technical date. This will be technical details. Yeah Yeah, anyways, I'm a nice. I know you could That's the technical details, right? So so Okay, I speak to this because after this we can summarize it from this so For okay, so we're have we found the project agreement yet So that would be to do so once that's available we need to sign that so it's probably sending on teams in range of sign it and The PO email we leave that to the end. We're discussing other stuff and about project understanding. It's just basically and We're back. That's compatible for both device like Windows device and mobile device and that should For us for demonstration purposes. It should have a UI so that we're assuming Ourself as the robot accessing the world website using the edge API entry points and we should draft out a What do you call that we should draft out a? so MVP that would be a to-do as well, so just
[10:24] So we need more cuts to the PO meeting? Do we have github setup?
[11:04] So yeah, could you share that at the end of the day today and make sure that's shared to GTAs and report should be set to private blah and Do you want me to set up the board? the JIRA board ? because I have a template
[11:22] I feel like everyone, because they are...
[11:27] which is for data quality of the product and we can start creating small stories. Scrum Master doesn't need to be on the board. Scrum Master is just there to facilitate the meetings so we don't go off topics. So we got Jira sorted.
[12:03] No, no, we need actual Jira. Like actual Jira, yeah, so Jira on the... Yeah, on that scene. We should all log in into that Jira? No, no, it's free. It's free. And I think we should all log in with the...
[12:20] University ID, yes, yes please. Yeah, University as well. So, oh yeah, make sure you GitHub, like your username has to be University ID, by the way, so your primary email.
[12:41] We said it at the get-go.
[12:43] Make sure that your GitHub handles underneath your name the primary email address has to be the UA email address or you won't get a grade. Just be careful of that. At the end of the product after we get marked, you won't get a mark if your main email address is not your UA email address. Make sure that it's your UA. Make sure GitHub was marked. We see about chicken and salt salt. Yeah. Also that.
[13:22] Thank you for the stand-up from the sitting time.
[13:34] I reckon just say discord, yeah.
[13:46] Maybe in the evening.
[13:49] Oh yeah, yeah. Just keep a meeting and everyone say hi and then...
[13:53] I feel like we should keep our weekly meetings as a stand-up meeting. So in the future, I assume we'll be doing... In college, there's a sprint planning. Yeah, yeah, yeah.
[14:09] Stand up? Once in a week we are booking a room for 1-2-3. We call it 1-2-3. Spring planning. And also, instead of this card, can we use Teams something? From home also we can connect with Cher and P ali.
[14:31] She actually wants to make it a company. Yeah, I see that.
[14:42] I mean this school you can join pools as well. Have you used Slack before? Same thing with Slack. For this school we will be...
[14:59] This is what I'm doing.
[15:01] You seen that call? So after you click join
[15:05] and there's a sharing screen and you can share your whole screen so it's like Slack so I reckon because we already made it the whole thing so I reckon with Sticking Discord
[15:18] Sorry? Here you can tell.
[15:21] schedule your meeting like. Yeah, yeah, you can also schedule your meeting. So yeah, that's fine.
[15:29] I'm just gonna go ahead and do that.
[15:30] I mean this course should be fine. This course should be fine.
[15:34] Yeah, you can sit up in it.
[15:38] Yeah, yeah, you can.
[15:46] It's all recorded in here. Yeah, yeah, yeah.
[16:12] Oh, so they're putting sprints as like a whole.
[16:21] It's a weekly sprint right? Sprints are weekly right for this one? Yeah, okay
[16:26] Yeah, so you need to have a ritual.
[16:32] Okay, yeah, that's fine.
[16:35] Yeah, yeah, it's only eight of us, yeah.
[16:40] That's what I'm saying right? Because product owners should be one of us. I think it's only for sprint reviews. So basically like a sprint planning.
[16:58] I think we put that as a to-do. So that's like, but we put that like, I mean the time for like, I mean one, two, three will be our basically meeting time. But like, like specifically what we do, we should discuss after the PO meeting.
[17:18] The meeting was a few.
[17:20] So whether, because we need to change that based on if he wants to join our meeting, then we need to change everyone's availability. Because we need to ask everyone, if you want preferred Monday, we prefer Monday at our clock, then we need to change that.
[17:41] During the lab session? Yeah. As I said. Because he said something about the labs being like a meeting. Okay.
[17:50] Depends on the food. Yeah, that's what I'm saying, depends.
[17:56] So you did the same projects as your powerful projects now, the same company now.
[18:02] I mean, that was sad.
[18:14] Do you know the PO's name? Yeah.
[18:17] I couldn't pronounce it properly.
[18:39] HOSO. Does he teach HCL?
[18:55] I don't know. Anyways.
[19:04] I can do you want me to set up the board for the jury? Yeah, okay. I will set up the board tonight as well Can we?
[19:12] Can you set up the GitHub? Yes. So you set up the GitHub, I'll set up the board.
[19:19] We've all understand what the project is doing. We have done our tech stack, which is React frontend. This is we're going to do a pool tonight, basically like basically a pool tonight saying what backend we're going to be using. So it's at a Node.js or Java with Spring.
[19:42] We have done our sort of like a stand-up schedule, right? So we're still just going to reserve this time, but you guys will be available during lifetime as well. I'll make my schedule around that, it should be fine.
[20:01] Sorry, for? Code reviews.
[20:09] I think we need to...so we need to pick four.
[20:13] So we need to stand up, code review, sprint review.
[20:19] and retrospective. I think ritual to be honest.
[20:28] Yeah, so we can put that as for now, right?
[20:32] Yeah, yeah, I feel like
[20:41] But I still feel like we need like a so whenever we make a PR we need to sort of we need to you need to ship you should be on like you should be like You should know where you we wrote you should have an understanding of what you basically did there You can't just one shot over there. That's my understanding so I feel like we should still have like a small like a short meeting was
[21:06] Did our professor ask us to have only four meetings?
[21:12] I have more than that only.
[21:15] This is kind of frame what?
[21:22] So it doesn't... I mean yeah... it's... yeah...
[21:28] Hmm, yeah, that's true, that's true. So, oh, so we're only looking at the sprint structure, right? Like, how we're gonna plan the sprint meetings, right? Is that what you were asking?
[21:41] So if it's sprint, like you're talking about the sprints about the structures, right? Other than that, yeah, we don't need code reviews for sprint structures, yeah.
[21:59] Yeah, we'll be our internal. We'll be on the...
[22:07] Yeah, yeah, yeah. My understanding was, you should be able to explain what you did there, and you should understand what you did. I literally review with my club. So I literally just ask my club, what has he done? And I understand, if it's fine then... Exactly. So I think in order for us to make sure that everyone else understands, so I feel like we should still do a meeting for PRs. You can use AI, whatever, just to understand it, but the person there presenting the PR should be able to tell everyone, basically, what is the architecture behind this.
[22:52] Yeah, exactly. It will be a peer review, right? Yeah, yeah, yeah. So just as long as the person is not pushing that by themselves, it's fine.
[23:01] Would that be fine? Yeah. Peer review? Nice.
[23:14] Yeah, I understand that, but...
[23:29] Yeah, that's the thing.
[23:31] But it is a bit weird, I understand that, because you always...
[23:36] industry you always make two separate same yeah won't be yeah because if you making changes on the front end
[23:49] You know, it's gonna screw up everyone. Yeah. Fuck.
[23:54] Should be fine. Yeah, no, because I have the same experience obviously you have. Yeah, true
[24:02] So this, the details like to the patient
[24:18] So you just have to create the blank schema at once in the Mongo, then it will be connected with your backend.
[24:25] API head goes on the data register window.
[24:29] Yeah, I think you can also hit from the front end now. Yeah.
[25:01] Especially for this one, I'll just say this for later on discussion, but still I think front-end should keep a track of what APIs you're making, what API you need, etc. In a PDF. Yeah, then you verify and do the test and then do the integration.
[25:23] I think that should be all.
[25:29] Are we missing anything? No, no, no. That should be alright.
[25:38] You can just put this time, so 1-2-3 as a fixed time schedule for all of us, if you need some sort of input for that.
[25:48] for the files you're going to submit.
[26:00] For retrospective, usually there's a general space for retrospective. And what you do is you just start the timer and it's like oh we did good, yeah, good, bad, improve, action, whatever, yeah, yeah.
[26:24] Yeah, we can. I mean, that's why for Jira, there's basically incognito mode. If you turn it on, everyone's incognito, so you can't see anyone. Anyone can see you as well.
[26:42] retrospective pages, it's always anonymous. Yeah, yeah, always. That's what I was saying.
[26:52] I mean, we can just show them the space. We can show them the space.
[26:57] If nobody posts something, we post it and then we have this issue and we solve it.
[27:03] Yeah, that's what I'm saying. I was like, yeah, I feel like, yeah, don't need to go in too deep. Yeah.
[27:17] So, okay, that should be fine.
[27:22] Yeah, yeah, go for it, go for it. I mean, I have it here, so I'll share it to the Discord afterwards.
[27:41] So it will be during this time.
[27:48] Tuesday this time. I think it's a good, what do you call it? It's a good time because it's not too late in the week and it's not too early in the week. So I think we can
[27:57] Yeah, and we don't have like our lectures on this thing.
[28:03] any changes so can you fix it before the demo.
[28:09] Ah, so you're saying that we can do an earlier day for the last week?
[28:18] for like the week before the demo, oh yeah for the week after the demo we could do like a Sunday or Monday we can just do online yeah Monday or Sunday we can just do online yeah we can just do online we have six prints, six official prints we don't think he will be online because he mentioned that he likes to meet in the university university? we will ask him, we'll ask him see his yeah sure we will do that
[28:49] Ah, don't. He socked.
[28:53] Shimura, I can send you the decision we made here afterwards and could you send Pio the email that just basically saying our tech stack and our specialized wall in one sentence like backhand, front hand. Oh, okay, then just basically our tech stack and just schedule a meeting with him. Because if we ask Christian, he's not going to email back to us, he's going to reply on the day.
[29:52] Is there anything like you hope to be able to do?
[30:00] Six sprints? Six sprints or seven sprints? I believe it's... Yeah, I think one sprint will be... I know it's week nine, we don't have one, right? Because of system 3.
[30:19] This week is week three, right? So this is project allocation. Next week will be sprint one. But I think sprint one will be a spike.
[30:30] The day said about Spring One will be a spike.
[30:35] Because that sprint one will be basically doing planning so we're not we shouldn't be doing this a spike Yeah, so sprint so week six will be the first assist demo yeah So week five will be sprint two we're gonna work on our project proposal basically what we want to do blah all that and then Next week will be a sprint planning so with the peel that makes sense. Oh, but the demos only start Wednesday week six
[31:07] That makes sense? Yeah, cool. And we have two sprints before that. Yeah. Basically. And this next week will be a spike sprint. Spike sprint basically we're not doing any coding. There's no code. Whatever. Yeah, it's just planning. And then we have week two, week three. Yeah. I think that should be all.
