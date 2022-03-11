<script>
  import Button from "./Button.svelte";
  import Badge from "./Badge.svelte";
  import Card from "./Card.svelte";
  import ButtonBagde from "./ButtonBagde.svelte";
  import Avatar from "./Avatar.svelte";
  import Footer from "./Footer.svelte";
</script>

<main>
  <section class="wrapper">
    <section class="ui">
      <section class="ting">
        <h2>Buttons</h2>
        <h4>Import buttons in your <code>{"<script>"}</code> tag</h4>
        <pre>
          <code>{`import Button from "./Button.svelte";`}</code>
        </pre>

        <section class="grid-ui">
          <section>
            <Button>default</Button>
            <pre>
            <code>{`<Button>default</Button>`}</code>
            </pre>
          </section>
          <section>
            <Button type="primary">primary</Button>
            <pre>
            <code>{`<Button type="primary">primary</Button>`}</code>
            </pre>
          </section>
          <section>
            <Button type="secondary">secondary</Button>
            <pre>
          <code>{`<Button type="secondary">secondary</Button>`}</code>
          </pre>
          </section>
          <section>
            <Button type="accent">accent</Button>
            <pre>
          <code>{`<Button type="accent">accent</Button>`}</code>
          </pre>
          </section>
          <section>
            <Button type="ghost">ghost</Button>
            <pre>
          <code>{`<Button type="ghost">ghost</Button>`}</code>
          </pre>
          </section>
          <section>
            <Button type="link">link</Button>
            <pre>
          <code>{`<Button type="link">link</Button>`}</code>
          </pre>
          </section>
        </section>
      </section>

      <section class="ting">
        <h2>Badges</h2>
        <h4>Import Badges in your <code>{"<script>"}</code> tag</h4>
        <pre>
          <code>{`import Badge from "./Bagde.svelte";`}</code>
        </pre>

        <section class="grid-ui">
          <section>
            <Badge>default</Badge>
            <pre>
             <code>{`<Badge>default</Badge>`}</code>
            </pre>
          </section>
          <section>
            <Badge type="primary">primary</Badge>
            <pre>
             <code>{`<Badge type="primary">primary</Badge>`}</code>
            </pre>
          </section>

          <section>
            <Badge type="secondary">secondary</Badge>
            <pre>
             <code>{`<Badge type="secondary">secondary</Badge>`}</code>
            </pre>
          </section>
          <section>
            <Badge type="accent">accent</Badge>
            <pre>
             <code>{`<Badge type="accent">accent</Badge>`}</code>
            </pre>
          </section>
          <section>
            <Badge type="ghost">ghost</Badge>
            <pre>
             <code>{`<Badge type="ghost">ghost</Badge>`}</code>
            </pre>
          </section>
          <section>
            <Badge type="border">Oulined</Badge>
            <pre>
             <code>{`<Badge type="border">Oulined</Badge>`}</code>
            </pre>
          </section>
        </section>
      </section>

      <section class="ting">
        <h2>Inbox Button</h2>
        <h4>Import inbox button in your <code>{"<script>"}</code> tag</h4>
        <pre>
          <code>{`import ButtonBadge from "./ButtonBagde.svelte";`}</code>
        </pre>

        <ButtonBagde title="Inbox" number="99+" />
        <pre>
          <code>{`<ButtonBagde title="Inbox" number="99+" />`}</code>
        </pre>
      </section>
    </section>

    <section class="card-avatar">
      <section class="ting">
        <h2>Card</h2>
        <h4>Import card in your <code>{"<script>"}</code> tag</h4>
        <pre>
          <code>{`import Card from "./Card.svelte";`}</code>
        </pre>
        <Card title="Shoes!" />
        <pre>
          
          <code>{`<Card title="Shoes!" />`}</code>
       </pre>
      </section>

      <section class="ting avatar">
        <h2>Avatar</h2>
        <h4>Import avatar in your <code>{"<script>"}</code> tag</h4>
        <pre>
          <code>{`import Avatar from "./Avatar.svelte";`}</code>
        </pre>
        <article class="sizes">
          <div>
            <Avatar type="large" name="K" />
            <pre>
          <code>{`<Avatar type="large"/>`}</code>
        </pre>
          </div>
          <div>
            <Avatar type="medium" name="K" image="false" />
            <pre>
          <code>{`<Avatar type="medium"/>`}</code>
        </pre>
          </div>
          <div>
            <Avatar type="small" name="K" />
            <pre>
          <code>{`<Avatar type="small"/>`}</code>
        </pre>
          </div>
        </article>
        <article class="sizes avatar">
          <div>
            <Avatar type="large" mode="indicator" name="K" />
            <pre>
          <code>{`<Avatar type="large" mode="indicator/>`}</code>
        </pre>
          </div>
          <div>
            <Avatar type="medium" name="K" image="false" />
            <pre>
          <code>{`<Avatar type="medium" mode="indicator/>/>`}</code>
        </pre>
          </div>
          <div>
            <Avatar type="small" name="K" />
            <pre>
          <code>{`<Avatar type="small" mode="indicator/>/>`}</code>
        </pre>
          </div>
        </article>
      </section>
    </section>
  </section>
</main>
<div class="foot">
  <h4>Import footer in your <code>{"<script>"}</code> tag</h4>
  <pre>
          <code>{`import Footer from "./Footer.svelte";`}</code>
        </pre>
  <pre>
          <code
      >{`<Footer
  links={["Branding", "Design", "Marketing", "Advertisement"]}
  links2={["About us", "Contact", "Jobs", "Press kit"]}
  links3={["Terms of use", "Privacy policy", "Cookie policy"]}
/>`}</code
    >
        </pre>
  <Footer
    links={["Branding", "Design", "Marketing", "Advertisement"]}
    links2={["About us", "Contact", "Jobs", "Press kit"]}
    links3={["Terms of use", "Privacy policy", "Cookie policy"]}
  />
</div>

<style>
  /* .avatar article {
    display: flex;
    gap: 1rem;
    margin-bottom: 1rem;
    align-items: end;
  } */

  /*   .grid-ui {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
  } */

  .foot h4,
  .foot pre {
    margin-left: 2rem;
  }

  main {
    display: grid;
    grid-template-columns: 10% 1fr 10%;
    justify-content: center;
  }

  .wrapper {
    grid-column-start: 2;
    justify-self: center;
    margin-top: 2rem;
    border-radius: 1rem;
    box-shadow: rgba(0, 0, 0, 0.4) 0px 30px 90px;
  }

  .ting {
    margin: 1rem 2rem;
  }

  .ting section {
    margin-top: 1rem;
  }

  h2 {
    margin-bottom: 1rem;
  }
</style>
