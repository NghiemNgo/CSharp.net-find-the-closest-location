# CSharp.net-find-the-closest-location

var latA = 21.0281814654153; // latitude
var lngA = 105.782892064078; // longtitude
var closestEvent = cnn.RequestFormUrls.Select(x => new { x.ID, delta = Math.Abs(x.Lati - latA) + Math.Abs(x.Long - lngA) }).OrderBy(x => x.delta).FirstOrDefault();
