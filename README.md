# ConfigurarGit

#Cambia Vi/Vim por Nano y Less por Cat

¡Hola que tal!

Más que un tutorial, quiero compartirte el comando para que git deje de usar Vi/Vim y en su lugar use Nano. Es útil cuando, por ejemplo, olvidas dejar el mensaje de un commit y git por defecto abre Vim para que puedas indicar el mensaje que olvidaste. Si no conoces los atajos ni la extraña forma que tiene Vim para funcionar, o simplemente porque prefieres nano para algo tan simple como indicar un mensaje olvidado, puedes cambiar esta configuración.

Para cambiarlo solo debes usar el siguiente comando en la terminal:

git config --global core.editor nano

Además, en Mac, al enviar un commit sin mensaje, al usar git log, git diff y otros, los resultados de estos comandos se muestran en una nueva página o vista y que luego debemos salir de esta para volver a la línea de comandos, lo que no ayuda cuando quieres copiar una referencia para hacer un checkout a un commit anterior o para ver diferencias. Esto es porque git por defecto abre less para estos resultados. Pero podemos cambiarlo por cat para que los resultados no aparezcan en nueva vista.

Para cambiarlo solo debes usar el siguiente comando en la terminal:

git config --global core.pager cat

Espero que les sea de utilidad.
