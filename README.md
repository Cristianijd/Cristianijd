#include <iostream>

using namespace std;

int main()
{
    int Mapamental,Exposicion,Evaluacion,Testintermedio,Laboratorio,Proyecto,Notatotal;
    const double pesoMapamental = 0.10; // 10%
    const double pesoExposicion = 0.10; // 10%
    const double pesoEvaluacion = 0.35; // 35%
    const double pesoTestintermedio = 0.15; // 15%
    const double pesoLaboratorio = 0.15;  // 15%
    const double pesoProyecto = 0.15;  // 15%
     double calificacionMapamental, calificacionExposicion,calificacionEvaluacion,calificacionTestintermedio,calificacionLaboratorio, calificacionProyecto;
    double promedioPonderado;

    // Solicitar calificaciones al usuario
    cout << "Ingresa la calificacion de Mapa mental: ";
    cin >> calificacionMapamental;

    cout << "Ingresa la calificacion de Exposicion: ";
    cin >> calificacionExposicion;

    cout << "Ingresa la calificacion de Evaluacion: ";
    cin >> calificacionEvaluacion;

    cout << "Ingresa la calificacion de Test intermedio: ";
    cin >> calificacionTestintermedio;

    cout << "Ingresa la calificacion de Laboratorio: ";
    cin >> calificacionLaboratorio;

    cout << "Ingresa la calificacion de Proyecto: ";
    cin >> calificacionProyecto;
     // Calcular el promedio ponderado
    promedioPonderado = (calificacionMapamental * pesoMapamental) +
                        (calificacionExposicion * pesoExposicion) +
                        (calificacionEvaluacion * pesoEvaluacion) +
                        (calificacionTestintermedio * pesoTestintermedio) +
                        (calificacionLaboratorio * pesoLaboratorio) +
                        (calificacionProyecto * pesoProyecto);
// Calcular nota final en escala de 100%
    double notaFinal = (promedioPonderado / 20) * 100;

    cout << "El promedio ponderado de tus calificaciones es: " << promedioPonderado << endl;
    cout << "La nota final en 100% es:" << notaFinal << endl;
    //Verificar si la nota final es menor que 14
    if(notaFinal< 14){
            cout<<"Resultado :Te quedas :( "<<endl;
    }else{
        cout<<"Resultado : Pasaste :) "<<endl;
    }
    return 0;
}

