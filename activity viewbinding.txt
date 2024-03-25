import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.yourapp.databinding.ActivityMainBinding // Replace with your binding class

class MainActivity : AppCompatActivity() {

    private lateinit var binding: ActivityMainBinding // Replace with your binding class

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityMainBinding.inflate(layoutInflater) // Inflate the binding
        setContentView(binding.root) // Set the root view from the binding

        // Access views using the binding object
        binding.rootLayout // Accesses the rootLayout from the layout XML
        binding.textView // Accesses a TextView with id "textView" from the layout XML

        // Example: Set text to a TextView using view binding
        binding.textView.text = "Hello, View Binding!"
    }
}
