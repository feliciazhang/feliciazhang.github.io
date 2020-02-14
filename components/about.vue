<template>
  <div id="about">
    <div class="about-description">
      <span class="about-description-strong">hey! 👋</span>
      thanks for stopping by. I'm a fourth year student at Northeastern University in Boston (Massachusetts born and raised!) where I'm studying computer engineering and computer science. currently, I'm at facebook as a software engineering intern, and previously at Drift ⚡, where I've been able to learn so much from so many talented people. I'm a fan of visuals, a good UI, and being able to really see how my work is impacting users so I focus on front end development, but I'm always down to learn to learn something new. when I'm not at the office or in the classroom, I'm also the outreach team lead for <a href="https://www.hackbeanpot.com" target="_blank">HackBeanpot</a>, a non profit organization that hosts an annual hackathon for Boston students to learn, grow, and get involved in the tech community.
    </div>

    <div class="about-important">
      <h3 class="about-important-title">a few things I care about</h3>
      <div class="about-important-item">
        <img src="~assets/icons/edu.svg" />
        <div class="about-important-details">
          <h3>education</h3>
          <p>
            you'll see that there's going to be a bit of a theme here about things that foster learning and expanding horizons and just overall gathering <span class="italics">more</span>. filling one's cup, per se. I'm so so priveleged to have access to some of the best education out there, to have channels for learning always be available to me, and everyone deserves to have that.
          </p>
        </div>
      </div>

      <div class="about-important-item">
        <img src="~assets/icons/lang.svg" />
        <div class="about-important-details">
          <h3>language</h3>
          <p>
            language is an amazing thing for the connections it creates between people and through time. it's so exciting to see that there's so much content and experience out there to learn from that becomes available to us because once a language barrier is crossed! so far, mandarin was my first language, I'm decents at german, and working on french.
          </p>
        </div>
      </div>

      <div class="about-important-item">
        <img src="~assets/icons/craft.svg" />
        <div class="about-important-details">
          <h3>making things</h3>
          <p>
            creating is just fun, whatever form it may be. my "making" manifests mostly in things like art and painting, knitting, sewing, baking etc. and of course, we can't forget about our good friend software dev. but the best part of making is seeing the results make someone else happy.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
  .about-description {
    text-align: justify;
    margin: 48px 132px;
    padding: 40px 100px;
    background-color: var(--main-red);
    color: var(--main-neutral);
    border-radius: 4px;
  }

  .about-description-strong {
    font-size: 28px;
    font-weight: bold;
  }

  .about-description a {
    color: var(--main-neutral);
  }

  .about-important {
    padding: 40px 232px;
    background-color: var(--main-pink);
    color: var(--main-navy);
    border-radius: 4px;
  }

  .about-important-title {
    font-family: var(--font-ovo);
    font-size: 28px;
    margin: 0 0 24px;
  }

  .about-important-item {
    display: flex;
  }

  .about-important-item img {
    width: 100px;
  }

  .about-important-details {
    margin: 0 0 16px 32px;
  }

  .about-important-item h3 {
    margin: 16px 0 8px;
    font-family: var(--font-ovo);
    font-size: 24px;
  }

  .about-important-item p {
    margin: 0;
    font-size: 14px;
    line-height: 20px;
    text-align: justify;
  }

  .italics {
    font-style: italic;
  }

  @media (max-width: 767px) {
    .about-description,
    .about-important {
      margin: 0;
      padding: 24px 16px;
    }

    .about-important-item {
      display: block;
      text-align: center;
    }

    .about-important-item img {
      width: 75px;
    }

    .about-important-details {
      margin-left: 0;
    }

    .about-important-item h3 {
      text-align: left;
    }
  }
</style>
