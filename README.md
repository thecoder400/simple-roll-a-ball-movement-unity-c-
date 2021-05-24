copy and paste the code under me



using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class playermovement : MonoBehaviour
{
    // this is a speed variable
    private float speed = 10;




    // Start is called before the first frame update
    void Start()
    {
        Debug.Log("subscribe to eldorado27");
        
    }

    // Update is called once per frame
    void Update()
    {
        float horizontal_movement = Input.GetAxis("Horizontal") * speed * Time.deltaTime;


        float vertical_movement = Input.GetAxis("Vertical") * speed * Time.deltaTime;





        transform.Translate(horizontal_movement, 0, vertical_movement);

    }
}
