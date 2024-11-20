<h1>Heading 1</h1>

# Heading 1

## Heading 2

### Heading 3

https://lesscss.org/functions/#math-functions

![Image not found](https://images.pexels.com/photos/170811/pexels-photo-170811.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

<img src="https://images.pexels.com/photos/170811/pexels-photo-170811.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"/>

| Name  | City  | Course |
| ----- | ----- | ------ |
| Rahul | Babra | WD     |

```css
/* #hero-section */

#hero-section {
  padding: var(--section-padding);
  padding-top: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: var(--bg-primary-color);
}

#hero-section > img {
  height: 400px;
}

#hero-section .content {
  max-width: 50%;
}

#hero-section .content h5 {
  color: var(--special-color);
}
#hero-section .content h2 {
  font-size: 48px;
}
#hero-section .content h4 {
  color: #1f7a31;
  font-weight: 400;
}
#hero-section .content p {
  margin-top: 10px;
  width: 80%;
  margin-bottom: 30px;
}

#hero-section .content span,
#about-me-section .content span {
  font-weight: 800;
  margin-left: 30px;
}
#hero-section .content span i,
#about-me-section .content span i {
  margin-left: 10px;
  color: var(--special-color);
}

/* #about-me-section */

#about-me-section {
  padding: var(--section-padding);
  margin-top: var(--section-gap);
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

#about-me-section > img {
  height: 600px;
}
#about-me-section .content {
  max-width: 50%;
}

#about-me-section .content > h4 {
  color: var(--special-color);
  font-weight: 600;
}
#about-me-section .content > h2 {
  font-size: 30px;
  font-weight: 500;
}
#about-me-section .content > p {
  margin: 15px 0px;
}

#about-me-section .content .details {
  margin-top: 20px;
  display: flex;
  align-items: center;
  gap: 30px;
  max-width: 80%;
  flex-wrap: wrap;
  margin-bottom: 30px;
}
#about-me-section .content .details .detail {
  display: flex;
}
#about-me-section .content .details .detail h3 {
  color: var(--special-color);
}
#about-me-section .content .details .detail img {
  height: 60px;
  margin-right: 10px;
}

/* #service-section */

#service-section {
  padding: var(--section-padding);
  margin-top: var(--section-gap);
}

#service-section .section-heading h6 {
  text-align: end;
  margin-right: 100px;
  color: var(--special-color);
}

#service-section .service-cards {
  margin-top: 30px;
  display: flex;
  justify-content: space-evenly;
}
#service-section .service-cards img {
  height: 250px;
}
#service-section .service-cards .service-card {
  max-width: 300px;
  text-align: center;
}

#service-section .service-cards .service-card h4,
#service-section .service-cards .service-card h5 {
  width: 100%;
  margin-top: 5px;
}
#service-section .service-cards .service-card h5 {
  font-weight: 400;
}
```

`ctrl+a`

### What is CSS ?

CSS stands for Cascading Style Sheets.

Here is example of card,

##### HTML

```html
<div class="card">
  <div class="header">
    <img
      src="https://images.pexels.com/photos/2379005/pexels-photo-2379005.jpeg?auto=compress&cs=tinysrgb&w=600"
      alt=""
    />
  </div>
  <div class="card-info">
    <h3>Rahul Baroliya</h3>
    <h4>Front End Developer</h4>
    <h5>Rajkot, Gujrat</h5>

    <div class="socials">
      <i class="fa-brands fa-linkedin"></i>
      <i class="fa-brands fa-github"></i>
      <i class="fa-solid fa-envelope"></i>
    </div>
    <button>Message</button>
  </div>
</div>
```

#### CSS

```css
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.card {
  max-width: 300px;
  border-radius: 24px;
  margin: 0 auto;
  margin-top: 50px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  overflow: hidden;

  transition: all 300ms;
}

.card .header {
  height: 100px;
  background-color: #555bf6;
  border-top-left-radius: inherit;
  border-top-right-radius: inherit;
  border: 1px solid transparent;
}

.card .header img {
  display: block;
  margin: 0 auto;
  margin-top: 30px;
  height: 100px;
  width: 100px;
  border-radius: 50%;
  object-fit: cover;
  border: 5px solid #555bf6;
}

.card .card-info {
  margin-top: 30px;
  padding: 15px;
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
  color: #aca199;
}

.card .card-info h3 {
  color: #3f3b39;
}
.card .card-info h5 {
  margin-top: 5px;
}

.socials {
  margin-top: 10px;
  font-size: 20px;
}

.socials i {
  margin-left: 10px;
}
.socials i:nth-child(1) {
  color: #2674b3;
}
.socials i:nth-child(2) {
  color: #5e5854;
}
.socials i:nth-child(3) {
  color: #bd6063;
}
button {
  margin-top: 15px;
  padding: 10px;
  border: none;
  outline: none;
  border-radius: 24px;
  background-color: #555afb;
  color: white;
  border: 2px solid transparent;

  transition: all 300ms;
}

button:hover {
  border: 2px solid #555afb;
  background-color: transparent;
  color: #555afb;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px
      30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
}

.card:hover .card-info {
  background-image: url(https://i.gifer.com/X5NS.gif);
}
```

![](CSS_CSS-3\Components\images\1699117921751.jpg)
