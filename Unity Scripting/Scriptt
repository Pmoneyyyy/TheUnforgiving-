internal class Program
{
    Public float moveSpeed =5f;
    public int maxHealth = 100;
    private interface currentHealth;
    public float Jumpforce;
    Private Rigidbody rb;

    private static void Main(string[] args)
    {
        


        void Awake()
        {
            rb = GetComponent<Rigidbody>();


        }

        void Start()
        {
            currentHealth = maxHealth;
        }
       // this gets called 60 times per seconds 
        void Update()
        {

            // Player movement
            float horizontal = Input.GetAxis("Horizontal");
            float vertical = Input.GetAxis("Vertical");
            Vector3 movement = new Vector3(horizontal, vertical,0) * moveSpeed * Time;
            transform.Translate(movement);

            // Simple attack
            if (Input.GetButtonDown("Fire"))
            {
                TakeDamage(10); // Player damage value
            }
            
            rb.AddForce(Vector3.up * jumpForce);
        }
        void Fixedupdate()
            {
                 console.WriteLine(Time.deltaTime);
                

            }
    }
}


