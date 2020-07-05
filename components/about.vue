<template>
  <div class="about" id="about">
    <div class="about-description">
      <span class="about-description-strong">hey! 👋</span>
      thanks for stopping by! I'm a student at Northeastern University in Boston where I'll be graduating with a degree in computer in 2021. most recently, I was at facebook as a software engineering intern, and previously at drift ⚡. I'm a fan of visuals, a nice UI, and being able to really see how my work is impacting users. I've mostly done front end web dev, but I'm always down to learn to learn something new. when I'm not at the office or in the classroom, I'm also the sponsorship team lead for <a href="https://www.hackbeanpot.com" target="_blank">HackBeanpot</a>, a non profit organization that hosts a hackathon for Boston students to learn, grow, and get involved in the tech community.
    </div>

    <div class="about-important">
      <h3 class="about-important-title">a few things I care about</h3>
      <div class="about-important-item">
        <img src="~assets/icons/edu.svg" />
        <div class="about-important-details">
          <h3>education</h3>
          <p>
            I've been so so lucky to have access to some of the best education out there, to have channels for learning always be available to me, and everyone deserves to have that.
          </p>
        </div>
      </div>

      <div class="about-important-item">
        <img src="~assets/icons/lang.svg" />
        <div class="about-important-details">
          <h3>language</h3>
          <p>
            language is a wonderful thing for the connections it creates between people and through time. it's amazing how many more worlds of information and experience can be opened up through language! so far, mandarin was my first language (just need to learn to read), I'm decent at german, and working on french.
          </p>
        </div>
      </div>

      <div class="about-important-item">
        <img src="~assets/icons/craft.svg" />
        <div class="about-important-details">
          <h3>making things</h3>
          <p>
            creating is just fun, whatever form it may be. my "making" manifests mostly in things like art and painting, sewing, baking etc. and of course, our good friend software dev. the process of having an idea and bringing it to its live form is super fun, but the best part of making is seeing the results make someone else happy.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
  .about {
    width: 900px;
    margin: 24px auto;
  }

  .about-description {
    text-align: justify;
    padding: 40px 88px;
    background-color: var(--main-red);
    color: var(--main-neutral);
    border-radius: 4px;
    margin-bottom: 48px;
  }

  .about-description-strong {
    font-size: 28px;
    font-weight: bold;
  }

  .about-description a {
    color: var(--main-neutral);
  }

  .about-important {
    color: var(--main-navy);
  }

  .about-important-title {
    font-family: var(--font-ovo);
    font-size: 28px;
    margin: 0 0 24px;
  }

  .about-important-item {
    display: flex;
    margin-bottom: 16px;
  }

  .about-important-item img {
    width: 100px;
  }

  .about-important-details {
    margin: 0 0 16px 48px;
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
