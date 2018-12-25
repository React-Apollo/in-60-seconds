---?color=linear-gradient(to bottom, #da9f5c, #dc778b)

# Let's  Started to Styled Components
[//]: <> (P1)
---

#### Add Some styled-components code

```javascript
const Button = styled.a`
  /* This renders the buttons above... Edit me! */
  display: inline-block;
  border-radius: 3px;
  padding: 0.5rem 0;
  margin: 0.5rem 1rem;
  width: 11rem;
  background: transparent;
  color: white;
  border: 2px solid white;

  /* The GitHub button is a primary button
   * edit this to target it specifically! */
  ${props => props.primary && css`
    background: white;
    color: palevioletred;
  `}
`

render(
  <div>
    <Button
      href="https://github.com/styled-components/styled-components"
      target="_blank"
      rel="noopener"
      primary
    >
      GitHub
    </Button>

    <Button as={Link} href="/docs" prefetch>
      Documentation
    </Button>
  </div>
)
```

[//]: <> (====P2====)
---?color=white
@title[Styled Components Basics]
@snap[ span-80]
@ul[spaced text-white]
- Automatic critical CSS
- No class name bugs
- Easier deletion of CSS
- Simple dynamic styling
- Painless Maintenance
- Automatic vendor prefixing
@ulend
@snapend


[//]: <> (P3)
---?color=white
@title[Installation]

#### Installation
use NPM
```bash
npm install --save styled-components
```
use Yarn
```bash
yarn add styled-components
```


[//]: <> (page4)

---


@snap[span-40 west] 
Getting Started
@snapend

@snap[ span-100]
 ```javascript
 // Create a Title component that'll render an <h1> tag with some styles
const Title = styled.h1`
  font-size: 1.5em;
  text-align: center;
  color: palevioletred;
`;

// Create a Wrapper component that'll render a <section> tag with some styles
const Wrapper = styled.section`
  padding: 4em;
  background: papayawhip;
`;

// Use Title and Wrapper like any other React component – except they're styled!
render(
  <Wrapper>
    <Title>
      Hello World!
    </Title>
  </Wrapper>
);
 ```
@snapend


