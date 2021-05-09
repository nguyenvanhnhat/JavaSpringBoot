# JavaSpringBoot
Spring MVC and REST Annotations

1. @Controller
  The @Controller is a class-level annotation. It is a specialization of @Component. 
  It marks a class as a web request handler. It is often used to serve web pages. 
  By default, it returns a string that indicates which route to redirect. 
  It is mostly used with @RequestMapping annotation.
 (@Controller là một chú thích cấp lớp. Nó là một chuyên môn hóa của @Component . 
  Nó đánh dấu một lớp là trình xử lý yêu cầu web. Nó thường được sử dụng để phục vụ các trang web. Theo mặc định, 
  nó trả về một chuỗi cho biết lộ trình chuyển hướng. Nó chủ yếu được sử dụng với chú thích @RequestMapping)

2. @RequestMapping: 
  It is used to map the web requests. 
  It has many optional elements like consumes, header, method, name, params, path, produces, and value. 
  We use it with the class as well as the method.
  (Nó được sử dụng để ánh xạ tới các yêu cầu web, Có thể chọn nhiều phần từ như consumes, header, method, name, params, path, produces, and value.
  Chúng ta sử dụng nó với các lớp như các phương thức)
  
3. @GetMapping: 
  It maps the HTTP GET requests on the specific handler method. 
  It is used to create a web service endpoint that fetches It is used 
  instead of using: @RequestMapping(method = RequestMethod.GET)
  (Nó ánh xạ các yêu cầu HTTP GET trên phương thức xử lý cụ thể. 
  Nó được sử dụng để tạo một điểm cuối dịch vụ web tìm nạp Nó được sử dụng 
  thay vì sử dụng:@RequestMapping(method = RequestMethod.GET))

4. @PostMapping:
  It maps the HTTP POST requests on the specific handler method. 
  It is used to create a web service endpoint that creates It is used 
  instead of using: @RequestMapping(method = RequestMethod.POST)
  (Nó ánh xạ các yêu cầu HTTP POST trên phương thức xử lí cụ thể.
  Nó được sử dụng để tạo một điểm cuối dịch vụ web tạo Nó được sử dụng 
  thay vì sử dụng: @RequestMapping (method = RequestMethod.POST)

5. @PutMapping: 
  It maps the HTTP PUT requests on the specific handler method.  
  It is used to create a web service endpoint that creates or updates It is used 
  instead of using: @RequestMapping(method = RequestMethod.PUT)
  (Nó ánh xạ các yêu cầu HTTP PUT trên phương thức xử lý cụ thể. 
  Nó được sử dụng để tạo một điểm cuối dịch vụ web tạo hoặc cập nhật Nó được sử dụng 
  thay vì sử dụng: @RequestMapping (method = RequestMethod.PUT)

6. @DeleteMapping: 
  It maps the HTTP DELETE requests on the specific handler method. 
  It is used to create a web service endpoint that deletes a resource. It is used 
  instead of using: @RequestMapping(method = RequestMethod.DELETE)
  (Nó ánh xạ các yêu cầu HTTP DELETE trên phương thức xử lý cụ thể. 
  Nó được sử dụng để tạo một điểm cuối dịch vụ web xóa tài nguyên. Nó được sử dụng 
  thay vì sử dụng: @RequestMapping (method = RequestMethod.DELETE))

7. @PatchMapping: 
  It maps the HTTP PATCH requests on the specific handler method. 
  It is used instead of using: @RequestMapping(method = RequestMethod.PATCH)
  (Nó ánh xạ các yêu cầu HTTP PATCH trên phương thức xử lý cụ thể. Nó được sử dụng 
  thay vì sử dụng: @RequestMapping (method = RequestMethod.PATCH))

8. @RequestBody: 
  It is used to bind HTTP request with an object in a method parameter. 
  Internally it uses HTTP MessageConverters to convert the body of the request. 
  When we annotate a method parameter with @RequestBody, 
  the Spring framework binds the incoming HTTP request body to that parameter.
  (Nó được sử dụng để liên kết yêu cầu HTTP với một đối tượng trong một tham số phương thức. 
  Bên trong nó sử dụng HTTP MessageConverters để chuyển đổi phần thân của yêu cầu. 
  Khi chúng ta chú thích một tham số phương thức với @RequestBody, 
  khung công tác Spring sẽ liên kết phần thân yêu cầu HTTP đến với tham số đó.)

9. @ResponseBody: 
  It binds the method return value to the response body. 
  It tells the Spring Boot Framework to serialize a return an object into JSON and XML format.
  ( Nó liên kết giá trị trả về của phương thức với phần thân phản hồi. 
  Nó yêu cầu Spring Boot Framework tuần tự hóa một đối tượng trả về thành định dạng JSON và XML.)

10. @PathVariable: 
  It is used to extract the values from the URI. 
  It is most suitable for the RESTful web service, where the URL contains a path variable. 
  We can define multiple @PathVariable in a method.
  (Nó được sử dụng để trích xuất các giá trị từ URI. Nó phù hợp nhất cho dịch vụ web RESTful, nơi URL chứa một biến đường dẫn. 
  Chúng ta có thể xác định nhiều @PathVariable trong một phương thức.)

11. @RequestParam: 
  It is used to extract the query parameters form the URL. 
  It is also known as a query parameter. It is most suitable for web applications. 
  It can specify default values if the query parameter is not present in the URL.
  (Nó được sử dụng để trích xuất các tham số truy vấn tạo thành URL. 
  Nó còn được gọi là tham số truy vấn . Nó phù hợp nhất cho các ứng dụng web. 
  Nó có thể chỉ định các giá trị mặc định nếu tham số truy vấn không có trong URL.)

12. @RequestHeader: 
  It is used to get the details about the HTTP request headers. 
  We use this annotation as a method parameter. 
  The optional elements of the annotation are name, required, value, defaultValue. 
  For each detail in the header, we should specify separate annotations. We can use it multiple time in a method
  (Nó được sử dụng để lấy thông tin chi tiết về tiêu đề yêu cầu HTTP. 
  Chúng ta sử dụng chú thích này như một tham số phương thức . 
  Các phần tử tùy chọn của chú thích là tên, bắt buộc, giá trị, giá trị mặc định. 
  Đối với mỗi chi tiết trong tiêu đề, chúng ta nên chỉ định các chú thích riêng biệt. 
  Chúng ta có thể sử dụng nó nhiều lần trong một phương thức.)

13. @RestController: 
  It can be considered as a combination of @Controller and @ResponseBody annotations. 
  The @RestController annotation is itself annotated with the @ResponseBody annotation. 
  It eliminates the need for annotating each method with @ResponseBody.
  (Nó có thể được coi là một sự kết hợp của @Controller và @ResponseBody chú thích . 
  Bản thân chú thích @RestController được chú thích bằng chú thích @ResponseBody. 
  Nó loại bỏ sự cần thiết phải chú thích từng phương thức với @ResponseBody.)

14. @RequestAttribute: 
  It binds a method parameter to request attribute. 
  It provides convenient access to the request attributes from a controller method. 
  With the help of @RequestAttribute annotation, we can access objects that are populated on the server-side.
  (Nó liên kết một tham số phương thức với thuộc tính yêu cầu. 
  Nó cung cấp quyền truy cập thuận tiện vào các thuộc tính yêu cầu từ một phương thức bộ điều khiển. 
  Với sự trợ giúp của chú thích @RequestAttribute, chúng ta có thể truy cập các đối tượng được điền ở phía máy chủ.)

