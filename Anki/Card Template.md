# Card Template

## Front

```
<div class="front-card">{{Word}}</div>

<div style="width: 300px; display: block; margin: 20px auto;">
	{{Photo}}
</div>
```

## Back

```
{{FrontSide}}

<hr id=answer>

<div class="back-card">
	{{Definition}}
</div>

<div class="context">
	{{Context}}
</div>
```

## Styling

```
body {
  margin-top: 50px;
}

.card {
  font-family: font-reg;
  font-size: 20px;
  text-align: center;
  color: black;
  background-color: white;

  /* ✅ Constrain readable width */
  max-width: 700px; /* adjust to taste: 600–800px is good for readability */
  margin: 0 auto; /* center the card horizontally */
  padding: 0 20px; /* add breathing room on the sides */
  box-sizing: border-box;
}

b,
strong {
  font-family: font-semibold;
}

.front-card {
  font-size: 24px;
  font-family: font-semibold;
  font-weight: 500;
}

.back-card {
  font-size: 20px;
  color: #344054;
}

ul > li {
  margin-top: 20px; /* Add margin to first-level <li> */
}

ul ul li {
  margin-top: 0; /* Remove margin from nested <li> */
}

.context {
  font-size: 18px;
  color: #344054;
  margin-top: 40px;
  text-align: left;
  line-height: 150%;
}

.nightMode .front-card {
  color: #fff;
}

.nightMode .back-card {
  color: #d0d5dd;
}

.nightMode .context {
  color: #d0d5dd;
}

.mobile .night_mode .front-card {
  color: #fff;
}

.mobile .nightMode .front-card {
  color: #fff;
}

.night_mode.card {
  color: #fff;
}

@font-face {
  font-family: font-reg;
  src: url("_Inter_18pt-Regular.ttf");
}

@font-face {
  font-family: font-medium;
  src: url("_Inter_18pt-Medium.ttf");
}

@font-face {
  font-family: font-semibold;
  src: url("_Inter_18pt-SemiBold.ttf");
}

@font-face {
  font-family: font-bold;
  src: url("_Inter_18pt-Bold.ttf");
}
```
