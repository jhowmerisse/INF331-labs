# Web Components

## Tarefa 1

## Tarefa 2

![codepen - web components](https://github.com/jhowmerisse/INF331-labs/blob/master/lab05%20-%20web%20components/images/Screenshot%20from%202020-08-31%2010-34-37.png)

### HTML

~~~~html
<div id="root"></div>
~~~~

### JS
~~~~js
const InputBox = () => {
  const [name, setName] = React.useState("Box");
  const [color, setColor] = React.useState("blue");
  const [size, setSize] = React.useState(111);

  return (
    <div className="input-box">
      <input
        type="text"
        placeHolder="nome"
        onChange={(e) => setName(e.target.value)}
      />

      <input
        type="number"
        placeHolder="tamanho em números"
        onChange={(e) => setSize(e.target.value)}
      />
      <select
        id="colors"
        name="color"
        onChange={(e) => setColor(e.target.value)}
      >
        <option value="red">red</option>
        <option value="purple">purple</option>
        <option value="blue" selected>
          blue
        </option>
        <option value="black">black</option>
      </select>
      <TextBox name={name} color={color} size={size} />
    </div>
  );
};

const TextBox = ({ name, color, size }) => (
  <span
    className="text-box"
    style={{ backgroundColor: `${color}`, width: `${size}px` }}
  >
    {name}
  </span>
);

const painel = (
  <div>
    <h1>Seja Bem vindo</h1>
    <h3>Modifique passando o nome, a largura e a cor desejada</h3>
    <InputBox />
  </div>
);

ReactDOM.render(painel, document.getElementById("root"));
~~~~

### CSS
~~~~css
body {
  background: #000;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
}

.text-box {
  color: white;
  margin-top: 5px;
  height: 50px;
  display: flex;
  box-shadow: gray 3px 2px 4px 1px;
  border-radius: 5px;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}

input {
  margin-right: 5px;
}

select {
  height: 21px;
  width: 70px;
}
~~~~
