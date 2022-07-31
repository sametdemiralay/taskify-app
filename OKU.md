- yarn create react-app ... --template typescript

- string tipinde bir useState oluşturup onun todo ve setTodo değerlerini props olarak bir component e verdiğinde o componentte aşağıdaki ikisinden birini yaparsın:


interface Props {
  todo: string;
  setTodo: React.Dispatch<React.SetStateAction<string>>;
}

const InputField = ({ todo, setTodo }: Props) => {...}

--- veya ---

const InputField:React.FC<Props> = ({ todo, setTodo }) => {...}
