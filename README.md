# graphql-service-client-Jwt


    $.ajax({
        url: "http://localhost:9000/api",
        contentType: "application/json",
        xhrFields: {
          withCredentials: true
        },
        type: "GET",
        data: '',
        success: function (response) {
          loginToken = response.token;
          $('#authStatus')
            .html("authenticated successfully")
            .css({ "color": "green", 'font-weight': 'bold' });
          $("#greetingDiv").html('').css({ 'color': '' });
        },
        error: (xhr, err) => alert('error')
      })
