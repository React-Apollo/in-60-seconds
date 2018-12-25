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

[//]: <> (P2)
---



<iframe src="https://codesandbox.io/embed/p55zy0301j?view=preview" style="width:100%; height:600px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>

