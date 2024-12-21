# Ex09 Event Registration Web Application
## Date:21-12-2006

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
# PAGE 1

<style>
  .competition-container {
    background-color: rgba(250, 253, 255, 1);
    display: flex;
    max-width: 480px;
    width: 100%;
    flex-direction: column;
    overflow: hidden;
    font-family: Inter, sans-serif;
    font-weight: 400;
    margin: 0 auto;
    padding: 41px 0 121px;
  }
  .header-wrapper {
    display: flex;
    width: 100%;
    flex-direction: column;
    font-size: 36px;
    color: rgba(0, 0, 0, 1);
    padding: 0 12px;
  }
  .logo-image {
    aspect-ratio: 6.67;
    object-fit: contain;
    object-position: center;
    width: 367px;
  }
  .competition-title {
    align-self: start;
    margin-left: 12px;
  }
  .competition-image {
    aspect-ratio: 0.86;
    object-fit: contain;
    object-position: center;
    width: 100%;
    margin-top: 45px;
  }
  .register-button {
    z-index: 10;
    background-color: rgba(188, 27, 27, 1);
    align-self: center;
    margin-top: 15px;
    width: 216px;
    max-width: 100%;
    font-size: 40px;
    color: rgba(255, 255, 255, 1);
    white-space: nowrap;
    padding: 4px 0 22px;
    border: none;
    cursor: pointer;
  }
  .register-button:hover,
  .register-button:focus {
    opacity: 0.9;
  }
  .register-button:focus {
    outline: 2px solid #000;
    outline-offset: 2px;
  }
</style>

<div class="competition-container">
  <div class="header-wrapper">
    <img
      loading="lazy"
      src="https://cdn.builder.io/api/v1/image/assets/5730e4467fb242c388229c7463028a93/00018444524c54cd14cbc3d110720ff96cdd9e080f9c42da15ea11ba56637112?apiKey=5730e4467fb242c388229c7463028a93&"
      class="logo-image"
      alt="Cube Competition Logo"
    />
    <h1 class="competition-title">CUBE COMPETITION</h1>
  </div>
  <img
    loading="lazy"
    src="https://cdn.builder.io/api/v1/image/assets/5730e4467fb242c388229c7463028a93/f7b7f7fddf93831ad3b817ce3a56473af5ed9431333c919a4be15c07b324626d?apiKey=5730e4467fb242c388229c7463028a93&"
    class="competition-image"
    alt="Cube Competition Featured Image"
  />
  <button class="register-button" tabindex="0">REGISTER</button>
</div>

#PAGE 2

<style>
  .events-container {
    background-color: rgba(91, 247, 250, 1);
    display: flex;
    max-width: 480px;
    width: 100%;
    flex-direction: column;
    overflow: hidden;
    color: rgba(0, 0, 0, 1);
    margin: 0 auto;
    padding: 48px 79px 338px 27px;
    font: 400 48px Inter, sans-serif;
  }

  .events-header {
    align-self: flex-start;
  }

  .events-list {
    align-self: flex-end;
    margin-top: 104px;
    width: 270px;
  }

  .visually-hidden {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect(0, 0, 0, 0);
    border: 0;
  }
</style>

<div class="events-container" role="region" aria-label="Events Section">
  <h1 class="events-header">EVENTS</h1>
  <nav class="events-list">
    <ul aria-label="Event Categories">
      <li>3x3</li>
      <li>2x2</li>
      <li>4x4</li>
      <li>5x5</li>
      <li>pyra</li>
      <li>3x3 OH</li>
    </ul>
  </nav>
</div>

#PAGE 3

<style>
.event-registration-container {
  background-color: rgba(49, 200, 255, 1);
  display: flex;
  max-width: 480px;
  width: 100%;
  flex-direction: column;
  overflow: hidden;
  margin: 0 auto;
  padding: 34px 19px 55px;
}

.form-title {
  color: rgba(0, 0, 0, 1);
  font: 400 36px Inter, sans-serif;
  align-self: start;
}

.input-field {
  background-color: rgba(217, 217, 217, 1);
  max-width: 100%;
  font: 400 36px Inter, sans-serif;
  color: rgba(0, 0, 0, 1);
}

.name-field {
  composes: input-field;
  width: 340px;
  margin: 58px 0 0 18px;
  padding: 0 6px 25px;
}

.gender-field {
  composes: input-field;
  width: 217px;
  margin: 39px 0 0 24px;
  padding: 9px 0;
}

.age-field {
  composes: input-field;
  width: 197px;
  margin: 58px 0 0 34px;
  padding: 7px 4px;
}

.reg-field {
  composes: input-field;
  width: 285px;
  align-self: center;
  margin-top: 67px;
  padding-bottom: 21px;
}

.mobile-field {
  composes: input-field;
  width: 259px;
  align-self: center;
  margin-top: 38px;
  padding: 0 2px 19px;
}

.email-field {
  composes: input-field;
  width: 330px;
  align-self: end;
  margin-top: 61px;
  padding: 2px 4px 16px;
}

.submit-button {
  background-color: rgba(249, 38, 38, 1);
  width: 309px;
  align-self: center;
  margin-top: 48px;
  padding: 15px 2px;
  color: rgba(255, 255, 255, 1);
  border: none;
  cursor: pointer;
  font: 400 36px Inter, sans-serif;
}

.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
</style>

<form class="event-registration-container">
  <h1 class="form-title">EVENT REGISTER FORM</h1>
  
  <label for="fullName" class="visually-hidden">Full Name</label>
  <input type="text" id="fullName" class="name-field" placeholder="FULL NAME" required>
  
  <label for="gender" class="visually-hidden">Gender</label>
  <select id="gender" class="gender-field" required>
    <option value="">GENDER</option>
    <option value="male">Male</option>
    <option value="female">Female</option>
    <option value="other">Other</option>
  </select>
  
  <label for="age" class="visually-hidden">Age</label>
  <input type="number" id="age" class="age-field" placeholder="AGE" required>
  
  <label for="regNo" class="visually-hidden">Registration Number</label>
  <input type="text" id="regNo" class="reg-field" placeholder="REG NO" required>
  
  <label for="mobile" class="visually-hidden">Mobile Number</label>
  <input type="tel" id="mobile" class="mobile-field" placeholder="MOB NO" required>
  
  <label for="email" class="visually-hidden">Email Address</label>
  <input type="email" id="email" class="email-field" placeholder="EMAIL ID" required>
  
  <button type="submit" class="submit-button">REGISTER</button>
</form>

#PAGE 4

<style>
.registration-container {
  background-color: rgba(255, 255, 255, 1);
  display: flex;
  max-width: 480px;
  width: 100%;
  flex-direction: column;
  overflow: hidden;
  color: rgba(0, 0, 0, 1);
  margin: 0 auto;
  padding: 32px 0 88px;
  font: 400 36px Inter, sans-serif;
}

.registration-image {
  aspect-ratio: 6.62;
  object-fit: contain;
  object-position: center;
  width: 100%;
}

.registration-message {
  align-self: start;
  margin: 605px 0 0 27px;
}

.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
</style>

<div class="registration-container" role="main" aria-label="Registration confirmation">
  <img
    loading="lazy"
    src="https://cdn.builder.io/api/v1/image/assets/5730e4467fb242c388229c7463028a93/dc533b27ce87e5ecd80e94cff82f9987ec6595730c2c39b315224f47a50fed61?apiKey=5730e4467fb242c388229c7463028a93&"
    class="registration-image"
    alt="Registration confirmation illustration"
  />
  <div class="registration-message" role="status" aria-live="polite">THANKS FOR REGISTERING !</div>
</div>
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/64fde6e4-f592-437c-9d61-32b96edbe6a2)

![image](https://github.com/user-attachments/assets/4a88e242-699a-4f45-94cb-6a2ca053b7fb)

![image](https://github.com/user-attachments/assets/eef4d4d1-a290-49d6-913b-8218b1783fc9)

![image](https://github.com/user-attachments/assets/ac5b2306-8da7-412c-9e8b-fec7bab3dbea)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
