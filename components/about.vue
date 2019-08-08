<template>
  <div id="about" class="about-container">
    <div class="about-description">
      <span class="about-description-strong">hey! 👋</span>
      thanks for stopping by. I'm a fourth year student at Northeastern University in Boston
      (Massachusetts born and raised!) where I'm studying computer engineering and computer science.
      currently, I'm a software engineering co-op at Drift ⚡, where I've been able to learn
      so much from so many talented people. I'm a fan of visuals, a good UI, and being able to really see
      how my work is impacting users so I focus on front end development, but I'm always down to learn
      to learn something new. when I'm not at the office or in the classroom, I'm also the outreach team lead for
      <a href="https://www.hackbeanpot.com" target="_blank">HackBeanpot</a>, a non profit organization
      that hosts an annual hackathon for Boston students to learn, grow, and get involved in the tech community.
    </div>

    <h3 class="about-important-title">a few things I care about</h3>
    <ul class="about-important-list">
      <li class="about-important-item">
        <h3>education</h3>
        <p>
          you'll see that there's going to be a bit of a theme here about things that foster learning and expanding
          horizons and just overall gathering <span class="italics">more</span>. filling one's cup, per se.
          education is at the center of growing one's knowledgebase. I'm so so priveleged to have access
          to some of the best education out there, to have channels for learning always be available to me,
          and everyone deserves to have that.
        </p>
      </li>

      <li class="about-important-item">
        <h3>language</h3>
        <p>
          language is an amazing thing for the connections it creates between people and even through time.
          knowing and understanding more languages increases those connections and opportunities for diverse
          experiences exponentially. there's just so much out there to discover and learn and for me language
          really facilitates that, which is why I love it. so far, mandarin was my first language, I'm passably
          good at german, and working on french.
        </p>
      </li>

      <li class="about-important-item">
        <h3>making things</h3>
        <p>
          creating is just fun, whatever form it may be. there's a reason why kids are always building towers
          and oragami hats and mud pies. my "making" manifests mostly in the form of 1800s pioneer housewife
          activities: art and painting, knitting, sewing, baking etc. and of course, we can't forget about
          our good friend software dev (considerably less 1800s). but the best part of making is giving it away
          and putting the results to good use.
        </p>
      </li>
    </ul>
  </div>
</template>

<style>
  .about-container {
    margin: 32px 132px;
    padding: 40px 100px;
    background-color: var(--main-red);
    color: var(--main-neutral);
    border-radius: 4px;
  }

  .about-description {
    text-align: justify;
  }

  .about-description-strong {
    font-size: 28px;
    font-weight: bold;
  }

  .about-description a {
    color: var(--main-neutral);
  }

  .about-important-title {
    font-family: var(--font-ovo);
    font-size: 28px;
    margin: 40px 0 24px;
  }

  .about-important-item h3 {
    margin: 16px 0 8px;
    font-family: var(--font-ovo);
  }

  .about-important-item p {
    margin: 0;
    font-size: 14px;
    line-height: 20px;
  }

  .italics {
    font-style: italic;
  }
</style>
