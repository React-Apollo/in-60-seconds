---?color=linear-gradient(to bottom, #da9f5c, #dc778b)

# Let's  Started to Styled Components

[//]: <> (P2)
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

[//]: <> (P3)
---



<iframe src="https://codesandbox.io/embed/p55zy0301j?view=preview" style="width:100%; height:600px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>

[//]: <> (P4)


---?color=#F6D365

@box[bg-orange text-white rounded demo-box-pad](Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.)

+++?color=black

@snap[north-west span-35]
@box[bg-green text-white demo-box-pad](1. Plan#Lorem ipsum dolor sit amet eiusmod)
@snapend

@snap[north-east span-35]
@box[bg-orange text-white rounded demo-box-pad](2. Build#Sed do eiusmod tempor labore)
@snapend

@snap[south-east span-35]
@box[bg-pink text-white demo-box-pad](3. Measure#Cupidatat non proident sunt in)
@snapend

@snap[south-west span-35]
@box[bg-blue text-white waved demo-box-pad](4. Repeat#Ut enim ad minim veniam prodient)
@snapend

@snap[midpoint]
@fa[refresh fa-3x]
@snapend