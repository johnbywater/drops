# Conversation with Ward

Ward: Whitehead's Process & Reality now in the federation: http://anw.fed.wiki/

Thompson: very cool

John: I noticed in the TOC, that section 3 of chapter is missing. Section 2 has "Section Hit" which is an OCR error in reading "Section III". So section 2 & 3 are together in the page for section 2.

I think it's very useful to have the TOC and the text in this way. When I'm reading the archive.com version, I never have any idea where I am, so I have never been able to locate something I read before by going to right section. I can normally recall a distinctive word phrase which is sufficient to narrow things down. But this wiki fixes that. The side-by-side way the wiki pages are presented works really well. Removing the hyphenation really helps too.

FYI The numbers that are scattered throughout are sometimes footnotes, but many of them are the page numbers in the original edition (this is the "corrected" edition).

The copy I was fixing up can be produced as an ebook, and has been, and ebook readers keep track of position and allow for notes. Whilst my original desire was to make something that would make it easier for friends to read, and I believe its being on archive.com is somehow legitimate, and whilst I don't want to discourage anything or act as the copyright police, this is a copyright work, and I didn't want to get into trouble with a publisher and so never actually circulated what I had made. My girlfriend at the time was also quite contemptuous of this little project, and told me that I don't need to spend week after week doing it when I can just buy myself a copy.

I also thought perhaps it would be better to go back to the original uncorrected edition. The original has the merit of having the slightly misremembered quotes from others, which Whitehead wrote down from memory without really checking. But I think that fits beautifully with the "subjective objectification" idea in his book: he wrote down what he thought they were, which represents what he cared to remember about these things. And going back to what somebody actually said kind of loses that quality. The "corrected" edition just replaced Whitehead's version of what people said with what they actually said, and I'm not sure if that's really an improvement, since anybody could just and find out what was actually said. The "corrected" edition also switches around closing single quotes and commas (as I noted before). As a programmer, I find this unhelpful. It might be conventional, but I prefer the original (I prefer 'one', and 'two' rather than 'one,' and 'two'). However, what the "corrected" edition did do, is unpick the changes which the publisher of the original edition added. This was a difficult task, since the original manuscript doesn't exist (it was burnt after Whitehead died), and was done by comparing two different first editions by two different publishers, who both slightly mangled what Whitehead wrote, in an attempt to be helpful. Apparently Whitehead's text didn't make as much sense to them as they thought it should have done, and so changed a few things. Whitehead himself wasn't really so interested in copy editing anyway, and so there was probably some room for improvements. And once you start improving one thing, then you can find yourself improving lots of other things. The other thing is that, although the original text would have gone out of copyright by now, it was actually extended by his wife, and so even the 90yrs old original is still in copyright (for another 20 or 30 years IIRC).

There is a book ("A Key to Whitehead's Process and Reality" by Donald W. Sherburne, published 1981) which reorganises the whole of Process and Reality on a topic-by-topic basis. This conforms with the more usual structure of a text book, but was a form that Whitehead didn't use, because he decided to adopt an incremental and iterative style, a style described by Whitehead (in the preface I think?) which deliberately spirals out from simple explanations, revisiting and refining topics as it makes its outward revolutions around the whole, unfolding the whole, as Christopher Alexander would recommend. This style is still quite unusual but it is also the style of another book that stood out for me: Anti-Oedipus by Deleuze and Guattari. Those two book, and Alexander's Timeless Way of Building are all remarkable similar books, and together have given me quite a lot of confidence to look at, and think about, things in the ways that are described and proposed in these books (and to avoid looking and thinking in the ways that are disregarded and criticised in these books). Timeless Way of Building relates to Pattern Language for Towns and Buildings in the same was as Anti-Oedipus relates to A Thousand Plateaus. I think both Alexander and Deleuze were influenced by Whitehead. But I've seen nothing in Deleuze that indicates he read Alexander's stuff, and I was told Alexander really didn't like the broad tradition in which D&G are often and perhaps wrongly positioned ("postmodernism"). Although, when I had dinner with Christopher Alexander in King's College SCR in Cambridge, a long fine dinner after which we were all very drunk, I was sitting next to him throughout, and ran quite a lot of D&G stuff past him, without making it obvious that's what I was doing, and he concurred with many things, and didn't object to anything, which wasn't surprising except for the reaction I had been warned to expect, since the concepts are similar to what he himself wrote). Anyway, the reason I mention "A Key To Whitehead's Process and Reality" is because it suggests the possibility to work on this "corrected" edition in a fully legitimate way, with explicit permission from the copyright holding publisher, to make a version or a derivative work, perhaps even just a distillation (but with many, very long quotes....) which is perhaps more accessible and useful for the purposes of it being read by people like us, by developers. there are academic philosophy types who seem to have done nothing of value with this work and are today having pointless arguments on Twitter about the status of this, that and the other, whether something is epistemological or ontological, who got that wrong, whether everything is conscious, and who needs laughing at now, which altogether seems both empty and neurotic. And the fact these people have salaries paid from by public money, and they seem to have produced nothing that I can use, when there seems so much to do, annoys a little bit.

My only other comment is that Whitehead's preface is actually a very useful introduction to the book. The first chapter of part one is a necessary introduction to the categories defined in chapter 2 (which is really where the system starts). But the preface kind of introduces the book as a whole, and indicates the game he is playing, the problem or context that the book is concerned with. The preface isn't included in this wiki. There is also an editor's preface, which is really boring, but it does describe quite well what they did, and why, and so you get an idea of the contributions they made to making this text what it is. The OCR errors you just have to use common sense about. If you see a particularly odd work (such as "coi implex") then just try to think of a normal word that got mangled by OCR (such as "complex"). Another example is "Section Hit" which is "Section III". Another is the OCR error "oncological principle" which should read "ontological principle" (Whitehead wasn't talking about the study and treatment of tumours).

I like this wiki, and the first way a publisher would raise an objection is through a cease and desist notice. So I guess it could continue until such time as a thing may appear? My feeling is that encouraging reading this largely unread text can only increase sales of the actual book. But they might take a different view. I'm really only sharing my own inhibitions, and was very pleased to see this wiki. I recognise it's not just a simple thing to do, and look forward to seeing whatever improvements may be made to it.

Ward: I started with the archive.org text as I think you could plainly see. I regret somewhat chopping that into separate files on part boundaries and separated the pieces I have omitted. I see after complaining about my own constructed table of contents that the work has a lot to say in its own table of contents.

I rushed this out without much double-checking so as to solicit your comments. Thanks for these.

Longer term, I just want to read the whole carefully and possibly index other work of my own that might follow. Do you have a lead on the original (uncorrected) text in machine readable form?

This is the script I used so far. I think I'll write a separate script for his table of context rather than confusing one script with both parsing tasks.


```
# translate parts i through v
# usage: ruby parts.rb

require 'json'

def asSlug title
  title.gsub(/\s/, '-').gsub(/[^A-Za-z0-9-]/, '').downcase
end

now = Time.now.to_i*1000

Dir.glob("text/*.part*.txt") do |filename|
  part = filename.sub(/text\/\d\d\./,'').sub(/\.txt/,'').sub(/\-/,' ').upcase
  text = File.read(filename)
  puts
  part = chapter = section = ''
  text.split(/^([A-Z ]+)$/).each_slice(2) do |body, sep|
    title = "#{part} #{chapter} #{section}".strip
      .sub(/PART/,'Part')
      .sub(/CHAPTER/,'Chapt')
      .sub(/SECTION/,'Sect')
      .sub(/DIAGRAMS/,'Diag')
      .gsub(/  +/,' ')
    unless sep.nil?
      if sep.match(/PART/)
        part = sep
        chapter = section = ''
      elsif sep.match(/CHAPTER/)
        chapter = sep
        section = ''
      elsif sep.match(/SECTION|DIAGRAMS/)
        section = sep
      else
        body = sep
      end
    end
    body = body.strip

    unless body.empty?
      puts "[[#{title}]]"
      page = {
        title: title,
        story: []
      }
      body.split(/\n\n/).each do |para|
        unless para.empty?
          page[:story].push({
            type: 'paragraph',
            text: para.gsub(/- *\n/,'').gsub(/\n/,' '),
            id: (rand()*10000000000000000).to_i.to_s
          })
        end
      end
      page['journal'] = [{
        type: 'create',
        item: page.dup,
        date: now
      }]
      File.open("/Users/ward/.wiki/white.localhost/pages/#{asSlug(title)}","w") do |file|
        file.puts JSON.pretty_generate(page)
      end
    end
  end
end
```

John: Nice code!

I did look (a good while ago) but couldn't find an OCR of the original edition. As I tried to say, my assessment was that it's probably beneficial to accept the changes made in the "corrected edition" since both the sprinkling of the original page numbers and the "trendy" ordering of commas and quotes are very superficial aspects compared with the extensive (and I'm sure greatly time consuming) expert scholarly work that must have been done to sift out what the publishers unfortunately adjusted in the original (the editors preface does detail the work they did). The page numbers can be stripped out, and the "quote-comma" syntax restored, and even restoring the original "botched" quotes wouldn't be such a strenuous task really (there aren't so many quotes in there). I would like to see how Whitehead remembered these quotes, I do feel that perhaps has some warmth which was lost in correcting him (but again perhaps it's better to use the original - I'm not a scholar). The academics (Griffin and Sherburne) that created this "corrected" edition are still alive, and are US citizens as far as I'm aware. Also the guy (Arthur Holmes, an Australian) who was teaching a course in this at Wheaton College in Chicago (videos on YouTube) is probably still around. So potentially they could be approached for advice? There's another academic (James R Williams) who I enjoyed spending time with at the Deleuze philosophy conference (2005 & 2006) who might be receptive to inquiries.

Ward: Section III in its proper place. Thanks.
http://anw.fed.wiki/view/welcome-visitors/view/process--reality/view/part-i-chapt-i-sect-iii

John: haha
I also spent time marking up the footnotes as footnotes, and marking up headings as headings, and guessing at what the OCR couldn't see. But, honestly, it's a long task! I did Part 1, and might have started Part 2, but it took a few weeks.
Regarding Whitehead's TOC - again, it's a time consuming task - it goes on and on, over several pages. But it is quite a neat little summary (map) of the whole thing.
Also the index at the back - it takes some editorial effort to make a good index for a book. So hyperlinking that back into the actual book would be very useful. I actually don't know if the ebook version (which is available for purchase) has these hyperlinks from the index or not. I should really buy a copy, as my ex-girlfriend contemptuously (but probably wisely) recommended.
https://www.amazon.co.uk/Process-Reality-Gifford-Lectures-Whitehead/dp/0029345707
Kindle edition: £8.99  🤣
(I don't think she fully appreciated that I was, more than anything, enjoying the nerdy geekery of working on this OCR-ed text to make an .epub file using tools designed for creating Python package documentation.)

Eric: "How do you choose to 'waste' your time?" is a good question for programmer ice-breakers and conversation-starters.

Ward: I spend three quarters of my waking hours programming and the rest I just waste.

I'm happier with my Whitehead Table of Contents which I had hoped would be done by noon. I know how to promote a few more phrases up to the upper levels and then I will be satisfied.

http://anw.fed.wiki/view/table-of-contents/view/part-i/view/part-i-chapt-i

John: That TOC works really well eh! I'm very impressed with this wiki :-)

Now you just have to read it! ;-)

Ward: http://anw.fed.wiki/view/table-of-contents/view/part-iii/view/part-iii-chapt-iii

John: It's looking good!

Here's somebody reading it out aloud into their laptop (aka "audio book")... This wasn't up when I was looking around ages ago, it's new on YouTube: https://www.youtube.com/watch?v=to9YDMXbBoU

I should admit, listening to this book being read out aloud whilst I was doing my housework/cooking/dishes was part of my motivation for making the ebook format. Although computer text-to-speech can be a bit tedious, the result wasn't actually all that bad. This YouTube video is obviously much nicer, being human voice. But really the best thing is just to read the actual text, and your wiki makes that a much better experience than anything else I've seen.

Ward: Now I will work on capitalization consistency

John: Hehe
FWIW, there's a pretty effective 1hr lecture on Process and Reality by Arthur Holmes on YouTube: https://www.youtube.com/watch?v=ysTx1c5-A7s&list=PL9GwT4_YRZdBf9nIUHs0zjrnUVl-KBNSM&index=61

But this is a North American current, to read Whitehead in the theology schools, they are Christians and there's this "process theology" thing which I personally find a bit odd. This lecture is in a Christian college, but it's pretty good at explaining the broad strokes of this work, and the resources Whitehead draws upon that aren't necessarily apparent from reading the text.

But he gets on the Process Theology in the next lecture. The one above isn't mixed up with that, it's quite good. This is the Process Theology lecture:
https://www.youtube.com/watch?v=Hwgoi0cvwmU&list=PL9GwT4_YRZdBf9nIUHs0zjrnUVl-KBNSM&index=62


Ward: Would you be willing to write some refections in a fork of this text? I'd love to get you set up to do that.

John: Yes I would. I just don't know really if I have so much to say.

Ward: I would expect you to talk about how particular ideas have influenced how you architect programs.
If you have 20 minutes to screen share, we can experiment with some possible formatting conventions for such reflections.

John: Well, I've probably only got two things to say about that.

1. The Python eventsourcing lib has "actual occasion" and "enduring object" as the base classes for "domain event" and "domain entity". That's here:
https://github.com/johnbywater/eventsourcing/blob/master/eventsourcing/whitehead.py
2. The "atomic" aspect of ACID DB transactions which makes writing records be an actual occasion (rather than an event that isn't an actual occasion, aka "dual writing"), situated within processing command and events in system. That is to say, dispensing with the notion of a continuous flow ("stream") in processing, so that we think of the running of software as an experience as a sequence of events, with the drops of experience being the "process events" that I diagrammed and wrote as a design pattern here and here:
https://eventsourcing.readthedocs.io/en/stable/topics/process.html#process-application
https://eventsourcing.readthedocs.io/en/stable/topics/process.html#process-event-pattern

Sure let's screen share! Please lead the way? What do you want me to do? Where do I go?

Mike: Wicked, Ward!

Sometimes I feel it would be satisfying and helpful to code. Then I return to ordinary language disciplines, ordinary skilful interactions, ordinary disciplined awareness - which, of course, are likewise extraordinary.

Takes mastery of all sorts!

Ward: I do enjoy coding and still learn new things about coding with every project. I understand that the skill is somewhat arcane much like copying morse code at conversational speeds or sailing across a downwind while rounding a buoy. I have all three skills but only one will pay in a day job though I can imagine when that might cease someday too. If one can think clearly and creatively and then use language to induce this in others, well, that is a skill that will remain in demand forever.