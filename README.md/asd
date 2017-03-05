$(window).load(function() {
  var linkl_list = [
    'https://drive.google.com/uc?export=download&id=[drive-id]'
  ];
  var update = function() {
    if (update_html) {
      var html = '';
      var drive_id = $('#driveID').val();

      $.each(linkl_list, function() {
        var drive_url = this.replace('[drive-id]', drive_id);
        html = html + '<div class="btn-group"><button type="button" class="btn btn-primary"><strong>Your Link:</strong></button><button type="button" class="btn btn-default"  contenteditable="true" onClick="document.execCommand(&quot;selectAll&quot;,false,null)">' + drive_url + '</button></div>';
      });
      $('#link_container').html(html);
    }
    update_html = false;
  }
  var update_html = true;

  $('#driveID').on('change', function() {
    update_html = true;
  });
  setInterval(update, 1000);
  update();
});

function getLink() {
  var e = document.getElementById("container");
  e.style.display = "block";
  var e = document.getElementById("get-button");
  e.style.display = "none";
};
$(function() {
  $('[data-toggle="tooltip"]').tooltip()
})
