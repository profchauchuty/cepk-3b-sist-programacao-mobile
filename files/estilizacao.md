# 🧾 Estilização no React Native

A tabela abaixo apresenta algumas das principais propriedades do `StyleSheet` do React Native, com descrição e exemplo de uso direto.

---

| Propriedade        | Descrição                                           | Exemplo                                        |
|--------------------|-----------------------------------------------------|------------------------------------------------|
| flex               | Define o espaço proporcional que o componente ocupa | container: { flex: 1 }                         |
| backgroundColor    | Define a cor de fundo do componente                 | header: { backgroundColor: '#FFF' }           |
| padding            | Espaçamento interno em todos os lados              | box: { padding: 16 }                           |
| margin             | Espaçamento externo em todos os lados              | box: { margin: 12 }                            |
| fontSize           | Define o tamanho da fonte do texto                 | title: { fontSize: 20 }                        |
| fontWeight         | Define a espessura da fonte                        | text: { fontWeight: 'bold' }                  |
| color              | Define a cor do texto                              | text: { color: '#333' }                        |
| borderWidth        | Define a espessura da borda                        | box: { borderWidth: 2 }                        |
| borderColor        | Define a cor da borda                              | box: { borderColor: '#000' }                   |
| borderRadius       | Arredonda os cantos do componente                  | button: { borderRadius: 8 }                    |
| width              | Define uma largura fixa                            | image: { width: 100 }                          |
| height             | Define uma altura fixa                             | image: { height: 100 }                         |
| alignItems         | Alinha itens no eixo transversal                   | container: { alignItems: 'center' }           |
| justifyContent     | Distribui itens no eixo principal                  | container: { justifyContent: 'space-between' } |
| textAlign          | Alinha texto dentro do componente                  | text: { textAlign: 'center' }                  |

---

## 💡 Exemplo

```js
import { View, Text, StyleSheet } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <Text style={styles.title}>Olá, mundo!</Text>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#F0F0F0',
    justifyContent: 'center',
    alignItems: 'center',
  },
  title: {
    fontSize: 24,
    color: '#333',
    fontWeight: 'bold',
  },
});
