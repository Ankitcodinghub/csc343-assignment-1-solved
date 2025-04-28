# csc343-assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [CSC343 Assignment 1 Solved](https://www.ankitcodinghub.com/product/csc343-goals-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;118005&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC343 Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
This assignment aims to help you learn to: read a relational scheme and analyze instances of the schema read and apply integrity constraints express queries and integrity constraints of your own think about the limits of what can be expressed in relational algebra

background

You will be working on a schema and queries for a database used by a zoological institute to track an archive of their artifacts.

During a eld trip collectors gather a variety of artifacts of the animals they study, resulting in tissue samples, images, physical models (such as casts of paw prints), or live colonies.

After arriving at the institute, artifacts must be safely stored and maintained by technicians. Some artifacts are cited in one or more publications. In all cases the o cial species name must be recorded, and must appear in the Catalogue of Life database. If correct taxonomic practices are followed, each species belongs to exactly one genus, and each genus to exactly one family. Tables COL, Genus, and Species are derived from Catalogue of Life database. relations

Collected(CID, AN)

Artifact(AN, species, type, location, SID)

Tuples here represent single artifact collected in the eld. AN is the artifact number, species is the scienti c species name, type is one of tissue, image, model, or live, location is where it was collected, and SID is the sta number of the technician who maintains this artifact.

COL(family)

A singleton tuple here means that family is a scienti c zoological family name that appears in the Catalogue of Life.

Genus(genus, family)

A tuple here means that genus is in family family.

Species(species, genus)

A tuple here means that species is in genus genus.

our constraints

For each of the following constraints give a one sentence explanation of what the constraint implies, and why it is required.

species(Artifact) species(Species) = ;. rank(Staff) f’technician’, ’student’, ’pre-tenure’, ’tenure’g.

family(Genus) family(COL) = ;. genus(Species) genus(Genus).

CID(Collected) = CID(Collection).

AN(Artifact) = AN(Collected).

SID(Collection) SID(Staff).

SID(Artifact) SID(Staff).

type(Artifact) f0tissue0;0 image0;0 model0;0 live0g

AN(Published) AN(Artifact)

queries

Write relational algebra expressions for each of the queries below. You must use notations from this course and operators:

In your queries pay attention to the following:

Do not make assumptions that are not enforced by our constraints above, so your queries should work correctly for any database that obeys our schema and constraints.

Other than constants such as 23 or “lupus”, a select operation only examines values contained in a tuple, not aggregated over an entire column.

Your selection conditions can use arithmetic operators, such as +; ;6=; ;&gt;;&lt; and friends. You can use logical operators such as _;^, and :, and treat dates and numeric attributes as numbers that you can perform arithmetic on.

Use good variable names and provide lots of comments to explain your intentions.

Return multiple tuples if that is appropriate for your query.

1. Rationale: Performance reviews include seeing how current the work is of sta who have held their current rank for a long time.

2. Rationale: Sta who maintain every artifact in some collection should be considered favourably in performance reviews.

Query: Find all sta who maintain all artifacts in at least one collection.

Query: Find all artifacts that were collected by the same sta who maintains them.

4. Rationale: Identify multi-talented eld workers.

Query: Find all sta who have collected at least 3 artifacts from every species in some family.

5. Rationale: Which publications might have some specialized niche focus?

Query: Find all publications that have used exactly 2 of our artifacts.

6. Rationale: Identify motherlode locations.

Query: Find all locations where at least one artifact from every family has been collected.

Query: Find all sta who have collected only tissue samples.

8. Rationale: Collection sta who should be encouraged to diversify their network.

Query: Find all sta pairs who have worked only with each other on collections.

9. Rationale: Track the in uence of a given sta member.

Query: Sta member SID1 is in uenced by sta member SID2 if (a) they have ever worked together on a collection or (b) if SID1 has ever worked with a sta member who is in uenced by SID2. Find SIDs of sta members in uenced by SID 42.

your constraints

1. No species is also a genus.

2. No genus belongs to more than one family.

3. All publications must be published after all artifacts they use have been collected.

Double check that you have submitted the correct version of your le by downloading it from MarkUs. marking

We mark your submission for correctness, but also for good form:

Please use the assignment operator, :=” for intermediate results.

Name relations and attributes in a manner that helps the reader remember their intended meaning.

Format the algebraic expressions with line breaks and formatting that help make the meaning clear.
